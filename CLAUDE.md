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

### 5. Lateralidad dinamica

La lateralidad se controla con un selector (Derecho/Izquierdo) y **nunca** debe estar hardcodeada en las plantillas. Usar siempre variables de lateralidad en lugar de escribir "derecho", "izquierdo", "DCHA", "IZQ", etc.

#### Variables de lateralidad disponibles

| Variable | Valor con "Derecho" | Valor con "Izquierdo" | Usar con sustantivos... |
|----------|--------------------|-----------------------|------------------------|
| `${LADO_M}` | derecho | izquierdo | masculinos minuscula: hombro, femur, humero, radio, codo, perone, muslo, brazo |
| `${LADO_F}` | derecha | izquierda | femeninos minuscula: rodilla, tibia, pierna, mano, clavicula, rotula, cresta iliaca, cadera |
| `${LADO_M_UPPER}` | DERECHO | IZQUIERDO | masculinos MAYUSCULA: FEMUR, HUMERO, RADIO, CODO, CARPIANO, MIEMBRO SUPERIOR |
| `${LADO_F_UPPER}` | DERECHA | IZQUIERDA | femeninos MAYUSCULA: RODILLA, TIBIA, MANO, ROTULA, CAR, PUC, CADERA |
| `${LADO_ABR_F}` | DCHA | IZDA | abreviatura femenina MAYUSCULA (solo PTC Summit/Zimmer: CADERA) |
| `${LADO_ABR_M}` | DCHO | IZDO | abreviatura masculina MAYUSCULA (osteotomias: MUSLO, FEMUR DISTAL) |
| `${DECUBITO}` | izquierdo | derecho | decubito lateral **contrario** (PTC y artroscopia hombro) |
| `${DECUBITO_UPPER}` | IZQUIERDO | DERECHO | decubito lateral contrario en MAYUSCULA |

#### Reglas de concordancia de genero

Elegir la variable segun el **genero gramatical** del sustantivo que la precede:

```
FRACTURA DE FEMUR ${LADO_M_UPPER}        ← femur es masculino → DERECHO/IZQUIERDO
RODILLA ${LADO_F_UPPER}                  ← rodilla es femenino → DERECHA/IZQUIERDA
Decubito lateral ${DECUBITO}             ← lado contrario → izquierdo/derecho
- Gonartrosis rodilla ${LADO_F}.         ← rodilla es femenino → derecha/izquierda
- Isquemia en muslo ${LADO_ABR_M}        ← muslo es masculino → DCHO/IZDO
```

#### `---` como placeholder generico

El placeholder `---` solo se debe usar cuando la lateralidad va junto a un sustantivo **masculino** y en minuscula (porque el sistema reemplaza `---` por "derecho"/"izquierdo" automaticamente). Para sustantivos femeninos o en mayusculas, usar **siempre** la variable explicita.

```
Artroscopia de hombro ---                ← OK: hombro es masculino, minuscula
Artroscopia de rodilla ${LADO_F}         ← OBLIGATORIO: rodilla es femenino
CAR ${LADO_F_UPPER}                      ← OBLIGATORIO: mayuscula + femenino
```

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

### 7. Estructura del archivo

- Archivo unico: `index.html`
- Array `CATEGORIAS` (~linea 668): definicion de categorias con `id`, `label`, `procs`
- Array `REGIONES` (~linea 782): agrupacion anatomica de categorias
- Funcion `obtenerPlantillas(DOCTOR, AYUDANTE, LADO)`: retorna objeto con todas las plantillas (LADO = 'D' o 'I')
- Cada plantilla tiene `hoja` (nota operatoria) y `tratamiento` (tratamiento al alta)

### 8. Al anadir una plantilla nueva

1. Anadir entrada en `CATEGORIAS[].procs` con `{ id, label }`
2. Anadir objeto `{ hoja, tratamiento }` en `obtenerPlantillas()`
3. El `hoja` debe empezar con `IQ ${FECHA} (${DOCTOR}/${AYUDANTE})` y usar formato con guiones (regla 2)
4. **Usar variables de lateralidad dinamica** (regla 5) — nunca hardcodear "derecho", "DCHA", "IZQ", etc. Elegir la variable segun el genero del sustantivo
5. El `tratamiento` debe usar formato con guiones e incluir `${DOCTOR}` en la revision
6. Actualizar `PLANTILLAS.md` con el contenido de la nueva plantilla
7. Verificar que el total de plantillas se incrementa correctamente
