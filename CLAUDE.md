# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Desarrollo

- **Abrir en navegador:** `open index.html` (no hay build, server ni dependencias)
- **No hay tests, linter ni CI** — verificar manualmente en navegador (Chrome + Safari iOS)
- **Diseño sistema B** (Clínico): fuentes Inter + Lora, ver `@STYLE-GUIDE.md` del repo padre

## Arquitectura del archivo único (`index.html`, ~6395 líneas)

| Sección | Líneas aprox. | Contenido |
|---------|--------------|-----------|
| Auth check | 4 | Redirect al hub si no autenticado (skip en localhost) |
| `<style>` | 25–1124 | CSS completo con dark mode (`[data-theme="dark"]`) |
| FAB "Envíanos tu plantilla" | 1127–1136 | Botón flotante inferior derecho (solo desktop), abre Gmail compose |
| `<script>` | 1465–6392 | Todo el JS vanilla |
| `CATEGORIAS[]` | 1469 | Array de 14 categorías con `id`, `label`, `procs[]` |
| `REGIONES[]` | 1590 | 5 regiones anatómicas que agrupan categorías |
| Utilidades | 1604+ | `normalizar()`, `hoy()`, `copiarTexto()` |
| `cargarPlantilla()` | 1616 | Orquesta selección quirófano → llama `obtenerPlantillas()` |
| `renderRegionPills()` | 1768 | Render de pills de región anatómica |
| `selectRegion()` | 1786 | Filtra categorías por región |
| `initTheme()` | 1988 | Dark mode toggle (sky CSS puro) |
| `selectModulo()` | 2026 | Cambia entre módulos Quirófano / Urgencias |
| `cargarPlantillaUrg()` | 2138 | Orquesta módulo urgencias |
| `obtenerPlantillas()` | 2413 | **Función central**: retorna objeto con todas las plantillas (`hoja` + `tratamiento`) |
| Plantillas | 2523–6390 | ~92 plantillas dentro de `obtenerPlantillas()` |

### Parámetros de `obtenerPlantillas(DOCTOR, AYUDANTE, LADO, ISQUEMIA, DRENAJE, FERULA)`

- `LADO`: `'D'` o `'I'` → genera todas las variables de lateralidad
- `ISQUEMIA`/`DRENAJE`/`FERULA`: booleanos → generan líneas condicionales en las plantillas

### Dos módulos

- **Quirófano**: navega por región → categoría → procedimiento → muestra hoja + tratamiento
- **Urgencias**: anamnesis + exploración + plan, con campos dinámicos (sexo, edad, lateralidad)

### Archivos de referencia

- `PLANTILLAS.md` (~221 KB): volcado de todas las plantillas — actualizar al añadir/modificar plantillas

---

# Plantillas Quirurgicas — Reglas del proyecto

## Reglas obligatorias para plantillas quirurgicas

Estas reglas se deben cumplir **siempre** al crear o modificar plantillas.

### 1. Header de nota operatoria

Toda plantilla debe empezar con:

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})
```

Seguido de una linea en blanco y el contenido de la intervencion.

**Nunca** incluir una linea `INTERVENCIÓN (DRS. ...)` — el header IQ ya contiene esa informacion.

### 2. Formato de la hoja operatoria

Las lineas de contenido de la `hoja` deben usar formato de listado con guiones (`- `):

- La primera linea tras la linea en blanco es el **titulo del procedimiento** → SIN guion
- Todas las lineas de contenido siguientes → CON guion `- `
- Lineas vacias se mantienen como separadores

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

Titulo del procedimiento ---
- Anestesia gral. + locorregional. Profilaxis ATB.
- Abordaje deltopectoral.
- Lavado, hemostasia, cierre por planos.
```

**Nunca** escribir lineas de contenido sin el prefijo `- `.

**Nunca** escribir contenido en MAYÚSCULAS enteras. Toda la hoja operatoria y el tratamiento deben usar formato en minúsculas (sentence case): primera palabra en mayúscula, resto en minúscula. Excepciones: abreviaturas médicas (LCA, CAR, DCP-LC, RAFI, TCS, SF, etc.), nombres de marca (Stryker, Zimmer, Tomofix, etc.), nombres de fármacos (METAMIZOL, PARACETAMOL, etc.) y encabezados de sección del tratamiento (CUIDADOS POSTOPERATORIOS, MEDICACIÓN, REVISIÓN, SÍNTOMAS DE ALERTA).

### 3. Revision en consulta

La linea de revision debe incluir **siempre** `${DOCTOR}`:

```
- Revision en CCEE de COT (${DOCTOR}) en X semanas para ...
```

**Nunca** hardcodear nombres de medicos ni fechas concretas (ej: `29/01/09`, `Dr. Lopez`).

### 4. Variables dinamicas

Usar siempre variables para datos que cambian por paciente:

| Variable | Uso |
|----------|-----|
| `${FECHA}` | Fecha de la intervencion (se rellena automaticamente) |
| `${DOCTOR}` | Cirujano principal |
| `${AYUDANTE}` | Ayudante de cirugia |

**Nunca** escribir valores fijos en lugar de estas variables.

### 5. Lateralidad dinamica

Ver reglas completas en `.claude/rules/lateralidad.md` (variables, concordancia de género, placeholder `---`).

**Nunca** hardcodear lateralidades como "derecho", "izquierdo", "DCHA", "IZQ", "DCHO", etc.

### 6. Key de plantilla

Formato `snake_case` con prefijo de categoria:

| Prefijo | Categoria |
|---------|-----------|
| `hombro_` | Artroscopia Hombro, Protesis Hombro |
| `codo_` | Codo |
| `ms_` | Miembro Superior |
| `rodilla_` | Rodilla (artroscopia, protesis, osteotomia) |
| `pie_` | Pie y Tobillo |
| `cadera_` | Cadera |
| `rpuc_` / `rpub_` | Recambio protesico |
| `tumores_` | Tumores |

### 7. Al anadir una plantilla nueva

1. Anadir entrada en `CATEGORIAS[].procs` con `{ id, label }`
2. Anadir objeto `{ hoja, tratamiento }` en `obtenerPlantillas()`
3. El `hoja` debe empezar con `IQ ${FECHA} (${DOCTOR}/${AYUDANTE})` y usar formato con guiones (regla 2)
4. **Usar variables de lateralidad dinamica** (regla 5) — nunca hardcodear "derecho", "DCHA", "IZQ", etc. Elegir la variable segun el genero del sustantivo
5. El `tratamiento` debe usar formato con guiones e incluir `${DOCTOR}` en la revision
6. Actualizar `PLANTILLAS.md` con el contenido de la nueva plantilla
7. Verificar que el total de plantillas se incrementa correctamente
