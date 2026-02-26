# 📋 Plantillas Quirurgicas COT

Aplicacion web de archivo unico para generar **notas operatorias** y **tratamientos al alta** en Cirugia Ortopedica y Traumatologia (COT). Disenada para agilizar la documentacion clinica en el dia a dia del quirofano.

![HTML5](https://img.shields.io/badge/HTML5-single--file-E34F26?logo=html5&logoColor=white)
![Plantillas](https://img.shields.io/badge/plantillas-87-1a3a5c)
![Regiones](https://img.shields.io/badge/regiones-5-16a34a)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-grey)

---

## Acceso directo

[Abrir la aplicacion](https://jmacot.github.io/plantillas-qx/)

No requiere instalacion. Funciona en cualquier navegador, incluyendo movil y tablet.

---

## Funcionalidades

- **87 plantillas quirurgicas** organizadas en 13 categorias y 5 regiones anatomicas (Trauma, Rodilla, Cadera, Miembro Superior, Pie y Tobillo)
- **Navegacion por regiones**: pills horizontales para filtrar por region anatomica
- **Campos dinamicos**: fecha del dia, cirujano y ayudante se insertan automaticamente en cada plantilla
- **Dos paneles simultaneos**: hoja operatoria (izquierda) y tratamiento al alta (derecha) con estilo glass y iconos SVG
- **Copia rapida** al portapapeles con un clic y confirmacion visual mediante toast animado
- **Diseno premium**: header con degradado, animaciones fadeInUp escalonadas y scrollbar personalizado
- **Modo oscuro / modo claro**: deteccion automatica por hora y sistema, con toggle manual
- **Archivo unico** (`index.html`): sin instalacion, sin servidor, sin dependencias

---

## Cómo usar

1. Descarga o clona el repositorio.
2. Abre `index.html` en tu navegador.
3. Escribe el **apellido del cirujano** y del **ayudante**.
4. Selecciona el **procedimiento** en el desplegable.
5. La hoja operatoria y el tratamiento al alta se generan automáticamente.
6. Pulsa **Copiar** y pega donde lo necesites (historia clínica, informe de alta, etc.).

---

## Catalogo de procedimientos

### Region: Trauma (13)

Canulados cadera, Gamma3, PPC Exeter, RAFI periprotesica NCB, RAFI supracondilea AXSOS, RAFI rotula cerclaje, Clavo T2 tibia, RAFI tobillo, Sutura Aquiles, RAFI EDR Aculoc-2, RAFI humero AxSOS, RAFI clavicula Variax, Monteggia Peri-Loc

### Region: Rodilla (36)

**Artroscopia (CAR)** — Mosaicoplastia, Fr meseta tibial, Reinsercion espina tibial, Ficat + plicatura ARI, SHER plicatura, Meniscectomia, Sutura meniscal, Artrolisis, Diagnostica, Cuerpo libre, Ficat, Toilette, Sinovectomia

**Protesis (PTR)** — Triathlon, PUC PKR, Revision PUC

**LCA** — ProCinch ST-RI, ProCinch ALL-INSIDE, ProCinch + Lemaire, ProCinch + sutura meniscal, ProCinch + reinsercion raiz, ALL-INSIDE Arthrex, HTH, Aumentacion AM, Aumentacion PL, Rescate revision, Rescate HTH banco + Lemaire

**Osteotomias y Cartilago** — CAR + OTV adiccion, CAR + OTV sustraccion Coventry, CAR + OTV varizante femur, OTV Tomofix, OVT apertura medial, OVT + correccion pendiente posterior, Fulkerson, Mosaico + OTV, LFPM + TTA

### Region: Cadera (3)

**Protesis (PTC)** — Summit DePuy, Zimmer G7 + Taperloc

**Artroscopia (CAC)** — Reinsercion labrum acetabular

### Region: Miembro Superior (30)

**Mano y Antebrazo** — STC, TCG mano, Dedo resorte A1, Dedo resorte tenolisis, RAFI EDR DVR, RAFI EDR ACUMED, Fr radio placa, Fr cubito + radio doble placa, Fr humero placa, Fr olecranon placa, Fr olecranon cerclaje, Seccion tendon flexor, Clavo T2 humero, Weaver-Dunn clavicula distal, Dupuytren, Ganglion mano, Infiltracion TMTC-STT, Rizartrosis trapeciectomia Welby

**Hombro** — CAH manguito rotador, CAH subescapular, Balon subacromial, CAH luxacion AC TwinBridge, PTHI Aequalis, PTHI Ascend, PTHI Biorsa, PTHI Revive, Elastofibroma dorsi

**Codo** — Biceps agudo, Biceps cronico, Epicondilitis

### Region: Pie y Tobillo (5)

Antepie, Pie plano osteotomia, Pie plano artrodesis, Pie cavo osteotomia, Pie cavo artrodesis

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
