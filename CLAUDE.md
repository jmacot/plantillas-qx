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

TITULO DEL PROCEDIMIENTO ---
- Anestesia gral. + locorregional. Profilaxis ATB.
- Abordaje deltopectoral.
- Lavado, hemostasia, cierre por planos.
```

**Nunca** escribir lineas de contenido sin el prefijo `- `.

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

### 5. Lateralidad

Usar `---` como placeholder editable para lateralidad (derecha/izquierda):

```
Artroscopia de hombro ---
```

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

### 7. Estructura del archivo

- Archivo unico: `index.html`
- Array `CATEGORIAS` (~linea 668): definicion de categorias con `id`, `label`, `procs`
- Array `REGIONES` (~linea 782): agrupacion anatomica de categorias
- Funcion `obtenerPlantillas(DOCTOR, AYUDANTE)`: retorna objeto con todas las plantillas
- Cada plantilla tiene `hoja` (nota operatoria) y `tratamiento` (tratamiento al alta)

### 8. Al anadir una plantilla nueva

1. Anadir entrada en `CATEGORIAS[].procs` con `{ id, label }`
2. Anadir objeto `{ hoja, tratamiento }` en `obtenerPlantillas()`
3. El `hoja` debe empezar con `IQ ${FECHA} (${DOCTOR}/${AYUDANTE})` y usar formato con guiones (regla 2)
4. El `tratamiento` debe usar formato con guiones e incluir `${DOCTOR}` en la revision
5. Actualizar `PLANTILLAS.md` con el contenido de la nueva plantilla
6. Verificar que el total de plantillas se incrementa correctamente
