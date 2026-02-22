# 📋 Plantillas Quirurgicas COT

Aplicacion web de archivo unico para generar **notas operatorias** y **tratamientos al alta** en Cirugia Ortopedica y Traumatologia (COT). Disenada para agilizar la documentacion clinica en el dia a dia del quirofano.

![HTML5](https://img.shields.io/badge/HTML5-single--file-E34F26?logo=html5&logoColor=white)
![Plantillas](https://img.shields.io/badge/plantillas-60-1a3a5c)
![Categorias](https://img.shields.io/badge/categorías-8-16a34a)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-grey)

---

## Acceso directo

[Abrir la aplicacion](https://jmacot.github.io/plantillas-qx/)

No requiere instalacion. Funciona en cualquier navegador, incluyendo movil y tablet.

---

## Funcionalidades

- **60 plantillas quirúrgicas** organizadas en 8 categorías, fieles a los documentos originales del servicio.
- **Campos dinámicos**: fecha del día, cirujano y ayudante se insertan automáticamente en cada plantilla.
- **Dos paneles simultáneos**: hoja operatoria (izquierda) y tratamiento al alta (derecha).
- **Copia rápida** al portapapeles con un clic y confirmación visual mediante banner animado.
- **Archivo único** (`notas_operatorias.html`): sin instalación, sin servidor, sin dependencias. Se abre en cualquier navegador.

---

## Cómo usar

1. Descarga o clona el repositorio.
2. Abre `notas_operatorias.html` en tu navegador.
3. Escribe el **apellido del cirujano** y del **ayudante**.
4. Selecciona el **procedimiento** en el desplegable.
5. La hoja operatoria y el tratamiento al alta se generan automáticamente.
6. Pulsa **Copiar** y pega donde lo necesites (historia clínica, informe de alta, etc.).

---

## Catálogo de procedimientos

### Trauma (13)
| Procedimiento |
|---|
| Canulados cadera — tornillos canulados (Stryker) |
| Clavo Gamma3 — Fr pertrocantérea cadera (Stryker) |
| PPC Exeter (Stryker) |
| RAFI Fr periprotésica cadera — Placa NCB (Zimmer) |
| RAFI Fr supracondílea fémur — Placa AXSOS (Stryker) |
| RAFI Fr rótula — cerclaje obenque (agujas K + alambre) |
| Clavo T2 tibia — fresado (Stryker) |
| RAFI Tobillo — placa baja energía peroné distal (Stryker) |
| Sutura tendón Aquiles (mini-open, Ma-Griffith) |
| RAFI Fr distal radio — Placa Aculoc-2 (Acumed) |
| RAFI Húmero proximal/diafisario — Placa AxSOS (Stryker) |
| RAFI Clavícula — Placa Variax (Stryker) |
| Fr Monteggia / olécranon — Placa Peri-Loc (S&N) |

### Artroscopia de Rodilla — CAR (17)
| Procedimiento |
|---|
| CAR Mosaicoplastia |
| CAR + Fr meseta tibial |
| CAR Reinserción avulsión espina tibial LCA |
| CAR Ficat + plicatura ARI (Lanny Johnson) |
| CAR SHER plicatura ARI + Ficat |
| CAR + OTV adicción |
| CAR + OTV sustracción (Coventry) |
| CAR + Osteotomía varizante fémur |
| OTV placa Tomofix (sin CAR) |
| CAR Meniscectomía parcial |
| CAR Sutura meniscal |
| CAR Artrolisis + movilización bajo anestesia |
| CAR Diagnóstica |
| CAR Extracción cuerpo libre |
| CAR Ficat |
| CAR Toilette |
| CAR Sinovectomía total |

### Prótesis de Cadera — PTC (2)
| Procedimiento |
|---|
| PTC Summit (DePuy) |
| PTC Zimmer (G7 + Taperloc) |

### Prótesis de Rodilla (3)
| Procedimiento |
|---|
| PTR Triathlon (Stryker) |
| PUC PKR (Stryker) |
| Revisión PUC (RPUC) |

### LCA — Stryker (5)
| Procedimiento |
|---|
| LCA ProCinch anatómico ST-RI |
| LCA ProCinch anatómico ALL-INSIDE |
| LCA ProCinch + Lemaire |
| LCA ProCinch + sutura meniscal |
| LCA ProCinch + reinserción raíz meniscal posterior |

### LCA — Otros / Revisión (6)
| Procedimiento |
|---|
| LCA ALL-INSIDE (Arthrex) |
| LCA Hueso-Tendón-Hueso (HTH) |
| LCA Aumentación AM |
| LCA Aumentación PL |
| LCA Rescate — revisión |
| LCA Rescate — HTH banco + Lemaire |

### Artroscopia de Cadera — CAC (1)
| Procedimiento |
|---|
| Reinserción labrum acetabular |

### Miembro Superior (13)
| Procedimiento |
|---|
| Síndrome del túnel carpiano (STC) |
| TCG Mano (quiste sinovial) |
| Dedo en resorte — apertura polea A1 |
| Dedo en resorte — tenolisis |
| RAFI Fr distal radio — Placa DVR |
| RAFI Fr distal radio — Placa ACUMED |
| Fr radio diafisario — placa |
| Fr cúbito + radio — doble placa |
| Fr húmero diafisario — placa |
| Fr olécranon — placa |
| Fr olécranon — cerclaje |
| Sección tendón flexor mano |
| Clavo T2 húmero retrógrado |

---

## Tecnología

- **HTML5 + CSS3 + JavaScript vanilla** en un solo archivo.
- Tipografías: [Inter](https://fonts.google.com/specimen/Inter) y [Lora](https://fonts.google.com/specimen/Lora) (Google Fonts).
- Sin frameworks, sin build tools, sin backend.
- Compatible con cualquier navegador moderno (Chrome, Firefox, Safari, Edge).

---

## Estructura del proyecto

```
plantillas-qx/
├── index.html        ← aplicacion completa (archivo unico)
├── icon.png          ← icono de la app
├── .gitignore
├── LICENSE           ← MIT
└── README.md         ← este archivo
```

---

## Licencia

MIT — Uso interno hospitalario. Contenido clinico basado en protocolos del servicio de COT.
