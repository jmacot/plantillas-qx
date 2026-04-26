# 📋 Plantillas COT

Mas de 100 notas operatorias y tratamientos al alta listos para usar. Elige el procedimiento, personaliza los datos y copia el texto directamente a la historia clinica. Incluye modulo de urgencias con anamnesis, exploracion y plan, y enlace directo al folleto postoperatorio personalizado.

![HTML5](https://img.shields.io/badge/HTML5-single--file-E34F26?logo=html5&logoColor=white)
![Plantillas](https://img.shields.io/badge/plantillas_qx-95-1a3a5c)
![Urgencias](https://img.shields.io/badge/plantillas_urg-7-dc2626)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-grey)

---

## Acceso

> Acceso protegido — requiere autenticacion previa desde el [portal principal](https://jmacot.github.io/).

[Abrir la aplicacion](https://jmacot.github.io/plantillas-qx/)

No requiere instalacion. Funciona en cualquier navegador, incluyendo movil y tablet.

---

## Modulos

### Quirofano

- **95 plantillas quirurgicas** organizadas en 14 categorias y 5 regiones anatomicas
- **Campos dinamicos**: fecha, cirujano, ayudante, lateralidad (D/I) y decubito se insertan automaticamente
- **Dos paneles**: hoja operatoria + tratamiento al alta
- **Toggle "Sutura meniscal"** en plantillas LCA para añadir o quitar la sutura sin cambiar de plantilla
- **Folleto postoperatorio personalizado** — boton al final del tratamiento abre `rehabilitacion-cot` con presets de injerto LCA y patron de menisco segun el procedimiento
- **Copia rapida** al portapapeles con un clic, con feedback visual de copiado

### Urgencias

- **Campos dinamicos**: sexo, edad, lateralidad, COT de guardia y tipo de tratamiento (conservador/quirurgico)
- **Tres paneles**: anamnesis, exploracion y plan de actuacion
- El texto se adapta automaticamente segun los campos seleccionados
- Categorias: Cadera, Rodilla, Tobillo, Muneca, Hombro (ampliable)

### FAB "Envianos tu plantilla"

- Boton flotante en la esquina inferior derecha (desktop) que abre Gmail compose pre-rellenado con el contexto de la plantilla activa, para sugerir mejoras o reportar erratas

---

## Como usar

1. Abre `index.html` en tu navegador.
2. Selecciona el **modulo** (Quirofano o Urgencias).
3. **Quirofano**: escribe cirujano/ayudante, selecciona la intervencion. Pulsa **Copiar** y pega donde lo necesites.
4. **Urgencias**: selecciona sexo, edad, lateralidad, conservador/quirurgico y diagnostico. Pulsa **Copiar**.

---

## Catalogo de procedimientos (Quirofano)

### Region: Trauma (13)

Canulados cadera, Gamma3, PPC Exeter, RAFI periprotesica NCB, RAFI supracondilea AXSOS, RAFI rotula cerclaje, Clavo T2 tibia, RAFI tobillo, Sutura Aquiles, RAFI EDR Aculoc-2, RAFI humero AxSOS, RAFI clavicula Variax, Monteggia Peri-Loc

### Region: Rodilla (44)

**Artroscopia (CAR, 17)** — Mosaicoplastia, Fr meseta tibial, Reinsercion espina tibial, Ficat + plicatura ARI, SHER plicatura, Meniscectomia, Sutura meniscal, Artrolisis, Diagnostica, Cuerpo libre, Ficat, Toilette, Sinovectomia, etc.

**Protesis (PTR, 5)** — Triathlon, PUC PKR, Revision PUC, **PUC Journey II UK (CORI)**

**LCA (14)** — ProCinch ST-RI, ProCinch ALL-INSIDE, ProCinch + Lemaire, ProCinch + sutura meniscal, ProCinch + reinsercion raiz, ALL-INSIDE Arthrex, HTH, **TightRope RF asimetrico**, Aumentacion AM, Aumentacion PL, Rescate revision, Rescate HTH banco + Lemaire

**Osteotomias y Cartilago (8)** — CAR + OTV adiccion, CAR + OTV sustraccion Coventry, CAR + OTV varizante femur, OTV Tomofix, OVT apertura medial, OVT + correccion pendiente posterior, Fulkerson, Mosaico + OTV, LFPM + TTA

### Region: Cadera (6)

**Protesis (PTC, 4)** — Summit DePuy, Zimmer G7 + Taperloc, **PTC Smith (CORI)**

**Artroscopia (CAC, 1)** — Reinsercion labrum acetabular

**Infiltracion (IFC, 1)**

### Region: Miembro Superior (30)

**Mano y Antebrazo** — STC, TCG mano, Dedo resorte A1, Dedo resorte tenolisis, RAFI EDR DVR, RAFI EDR ACUMED, Fr radio placa, Fr cubito + radio doble placa, Fr humero placa, Fr olecranon placa, Fr olecranon cerclaje, Seccion tendon flexor, Clavo T2 humero, Weaver-Dunn clavicula distal, Dupuytren, Ganglion mano, Infiltracion TMTC-STT, Rizartrosis trapeciectomia Welby

**Hombro** — CAH manguito rotador, CAH subescapular, Balon subacromial, CAH luxacion AC TwinBridge, PTHI Aequalis, PTHI Ascend, PTHI Biorsa, PTHI Revive, Elastofibroma dorsi

**Codo** — Biceps agudo, Biceps cronico, Epicondilitis

### Region: Pie y Tobillo (5)

Antepie, Pie plano osteotomia, Pie plano artrodesis, Pie cavo osteotomia, Pie cavo artrodesis

---

## Diagnosticos de Urgencias

- **Cadera**: Fr subcapital, Fr pertrocanterea
- **Rodilla**: Rotura LCA, Lesion meniscal
- **Tobillo**: Fr tobillo, Esguince tobillo
- **Muneca**: Fr radio distal, Fr escafoides
- **Hombro**: Luxacion hombro, Fr humero proximal

---

## Tecnologia

- **HTML5 + CSS3 + JavaScript vanilla** en un solo archivo (Sistema B "Radiologia Glass").
- Tipografias: Source Serif 4 + Source Sans 3 + Source Code Pro (Google Fonts).
- Glassmorphism con `backdrop-filter`, mesh gradient animado de fondo y sky toggle CSS puro para modo oscuro.
- Accesibilidad: skip link, focus-visible, smooth scroll, reduced-motion, aria-labels.
- Sin frameworks, sin build tools, sin backend.
- Compatible con cualquier navegador moderno (Chrome, Firefox, Safari, Edge).

---

## Licencia

All Rights Reserved — Uso interno hospitalario. Contenido clinico basado en protocolos del servicio de COT.
