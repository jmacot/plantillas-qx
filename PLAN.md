# Plan: Reestructurar la app en 3 secciones principales

## Objetivo
Dividir la aplicación en **3 módulos de nivel superior** que se seleccionan al entrar:
1. **Quirófano** — Lo que ya existe (plantillas operatorias + tratamiento al alta)
2. **Urgencias** — Nuevo: plantillas de urgencias con campos dinámicos
3. **Recomendaciones** — Nuevo: sección futura (esqueleto preparado)

---

## Paso 1 — Navegación principal de nivel superior (módulos)

**Qué se hace:**
- Añadir una barra de navegación principal **encima** de las region pills actuales, con 3 botones grandes (módulos): `Quirófano`, `Urgencias`, `Recomendaciones`.
- Estilo visual: pills grandes con iconos SVG diferenciados (bisturí, cruz urgencias, documento).
- Al cargar la app, se muestra esta barra y **ningún módulo seleccionado** (pantalla de bienvenida) o bien Quirófano activo por defecto.

**Cambios en el código:**
- Nueva constante `MODULOS` con `[{id, label, icon}]`
- Nueva función `selectModulo(moduloId)` que muestra/oculta las secciones correspondientes
- Variable de estado `activeModulo`
- El HTML del `<nav class="cat-nav">` se envuelve en un contenedor de sección `quirofano-section`

**Archivos:** `index.html` (HTML + JS)

---

## Paso 2 — Encapsular Quirófano como sección

**Qué se hace:**
- Envolver todo el contenido actual (region pills, subcat pills, formulario, paneles de texto) dentro de un `<div id="seccion-quirofano">` que se muestra/oculta según el módulo activo.
- No se cambia nada de la lógica interna de Quirófano — sigue funcionando exactamente igual.

**Cambios:**
- Mover `regionPills`, `subCatPills`, el `.card` del formulario y la `.panels-grid` dentro de `<div id="seccion-quirofano" style="display:none">`
- `selectModulo('quirofano')` → muestra esa sección, oculta las otras

**Archivos:** `index.html` (HTML)

---

## Paso 3 — Crear sección Urgencias (estructura y formulario)

**Qué se hace:**
- Crear `<div id="seccion-urgencias" style="display:none">` con:
  - **Pills de categoría** (diagnósticos de urgencias, ej. "Fr cadera", "Fr muñeca", etc.) — se llenarán cuando subas los archivos
  - **Formulario con campos dinámicos:**
    - **Sexo**: desplegable `Hombre / Mujer`
    - **Edad**: campo numérico (input number)
    - **Lateralidad**: desplegable `Derecho / Izquierdo`
    - **Tipo de tratamiento**: desplegable `Conservador / Quirúrgico`
    - **Diagnóstico**: desplegable con la lista de patologías (se puebla al seleccionar categoría)
  - **3 paneles de texto** (en vez de 2):
    - **Anamnesis** — se rellena dinámicamente con sexo, edad, lateralidad
    - **Exploración** — se rellena dinámicamente con sexo, edad, lateralidad
    - **Plan** — se rellena según conservador/quirúrgico

**Layout de paneles:**
- Desktop: 3 columnas (anamnesis | exploración | plan)
- Móvil: apilados verticalmente
- Cada panel con su botón "Copiar" (igual que ahora)

**Archivos:** `index.html` (HTML + CSS + JS)

---

## Paso 4 — Motor de plantillas para Urgencias

**Qué se hace:**
- Nueva estructura de datos `URGENCIAS_PLANTILLAS`:

```javascript
const URGENCIAS_CATEGORIAS = [
  { id: 'urg_cadera', label: 'Fr Cadera', procs: [
    { value: 'urg_fr_cadera_subcap', label: 'Fr subcapital cadera' },
    // ...
  ]},
  // ...más categorías
];

// Cada plantilla de urgencias:
urg_fr_cadera_subcap: {
  anamnesis: (sexo, edad, lado) => `Paciente ${sexo === 'M' ? 'varón' : 'mujer'} de ${edad} años que acude a urgencias por dolor en cadera ${lado} tras caída casual...`,
  exploracion: (sexo, edad, lado) => `Impotencia funcional de MII ${lado}. Acortamiento y rotación externa de la extremidad ${lado}...`,
  plan_conservador: (sexo, edad, lado) => `Tratamiento conservador: tracción cutánea...`,
  plan_quirurgico: (sexo, edad, lado) => `Plan quirúrgico: Se programa para intervención quirúrgica...`
}
```

- Las plantillas usan **funciones** en lugar de template literals estáticos, recibiendo (sexo, edad, lado) como parámetros
- `cargarPlantillaUrgencias()` lee los 4 campos del formulario y genera los 3 textos
- El campo "tipo de tratamiento" determina cuál plan se muestra

**Archivos:** `index.html` (JS)

---

## Paso 5 — Crear sección Recomendaciones (esqueleto)

**Qué se hace:**
- Crear `<div id="seccion-recomendaciones" style="display:none">` con:
  - Mensaje placeholder: "Próximamente — Recomendaciones postoperatorias"
  - Estructura preparada para futura expansión (pills + panel de texto)
  - Mismo estilo visual que las otras secciones

**Archivos:** `index.html` (HTML)

---

## Paso 6 — CSS para los nuevos componentes

**Qué se hace:**
- Estilos para la barra de módulos (`.modulo-pills`): pills más grandes, iconos, colores diferenciados
- Grid de 3 columnas para los paneles de Urgencias (`.panels-grid-3`)
- Colores diferenciados por módulo (ej. Urgencias en rojo/naranja, Recomendaciones en verde)
- Formulario de Urgencias: layout de 5 campos en fila (responsive a 2 filas en móvil)
- Dark mode: las variables CSS ya existentes cubren los nuevos elementos

**Archivos:** `index.html` (CSS)

---

## Paso 7 — Actualizar header y footer

**Qué se hace:**
- Título: "Plantillas COT" (más genérico, ya no solo quirúrgicas)
- Subtítulo dinámico según módulo activo
- Footer: actualizar versión a v4.0
- README y PLANTILLAS.md: actualizar con la nueva estructura

**Archivos:** `index.html`, `README.md`

---

## Paso 8 — Poblar plantillas de Urgencias

**Qué se hace:**
- Cuando subas los archivos de urgencias, incorporar cada diagnóstico en la estructura `URGENCIAS_PLANTILLAS`
- Cada entrada con sus 4 campos: anamnesis, exploración, plan conservador, plan quirúrgico
- Adaptar los textos para que usen las variables dinámicas (sexo, edad, lateralidad)

**Nota:** Este paso se hará cuando proporciones los archivos.

---

## Resumen de la arquitectura final

```
App
├── [Módulo] Quirófano          ← lo actual, sin cambios internos
│   ├── Región pills (Trauma, Rodilla, ...)
│   ├── Subcategoría pills
│   ├── Formulario (cirujano, ayudante, intervención)
│   └── 2 paneles (Hoja Operatoria + Tratamiento al Alta)
│
├── [Módulo] Urgencias           ← nuevo
│   ├── Categoría pills (diagnósticos de urgencias)
│   ├── Formulario (sexo, edad, lateralidad, conservador/quirúrgico, diagnóstico)
│   └── 3 paneles (Anamnesis + Exploración + Plan)
│
└── [Módulo] Recomendaciones     ← nuevo (esqueleto)
    └── (estructura preparada para futuro)
```

## Orden de implementación

Se puede hacer en fases:
- **Fase 1** (pasos 1-2-5-6-7): Estructura de módulos + encapsular Quirófano + esqueleto Recomendaciones → app funcional con la nueva navegación
- **Fase 2** (pasos 3-4): Sección Urgencias con formulario y motor de plantillas
- **Fase 3** (paso 8): Poblar plantillas cuando subas los archivos
