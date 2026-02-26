# 📋 Plantillas COT

Aplicacion web de archivo unico para **Cirugia Ortopedica y Traumatologia (COT)** con tres modulos: **Quirofano** (notas operatorias y tratamientos al alta), **Urgencias** (anamnesis, exploracion y plan con campos dinamicos) y **Recomendaciones** (proximamente). Disenada para agilizar la documentacion clinica.

![HTML5](https://img.shields.io/badge/HTML5-single--file-E34F26?logo=html5&logoColor=white)
![Plantillas](https://img.shields.io/badge/plantillas_qx-87-1a3a5c)
![Urgencias](https://img.shields.io/badge/plantillas_urg-10-dc2626)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-grey)

---

## Acceso directo

[Abrir la aplicacion](https://jmacot.github.io/plantillas-qx/)

No requiere instalacion. Funciona en cualquier navegador, incluyendo movil y tablet.

---

## Modulos

### Quirofano

- **87 plantillas quirurgicas** organizadas en 13 categorias y 5 regiones anatomicas
- **Campos dinamicos**: fecha, cirujano y ayudante se insertan automaticamente
- **Dos paneles**: hoja operatoria + tratamiento al alta
- **Copia rapida** al portapapeles con un clic

### Urgencias

- **Campos dinamicos**: sexo, edad, lateralidad y tipo de tratamiento (conservador/quirurgico)
- **Tres paneles**: anamnesis, exploracion y plan de actuacion
- El texto se adapta automaticamente segun los campos seleccionados
- Categorias: Cadera, Rodilla, Tobillo, Muneca, Hombro (ampliable)

### Recomendaciones

- Proximamente — seccion preparada para recomendaciones postoperatorias y protocolos

---

## Como usar

1. Abre `index.html` en tu navegador.
2. Selecciona el **modulo** (Quirofano, Urgencias o Recomendaciones).
3. **Quirofano**: escribe cirujano/ayudante, selecciona la intervencion.
4. **Urgencias**: selecciona sexo, edad, lateralidad, conservador/quirurgico y diagnostico.
5. Los textos se generan automaticamente.
6. Pulsa **Copiar** y pega donde lo necesites.

---

## Catalogo de procedimientos (Quirofano)

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

## Diagnosticos de Urgencias

- **Cadera**: Fr subcapital, Fr pertrocanterea
- **Rodilla**: Rotura LCA, Lesion meniscal
- **Tobillo**: Fr tobillo, Esguince tobillo
- **Muneca**: Fr radio distal, Fr escafoides
- **Hombro**: Luxacion hombro, Fr humero proximal

---

## Tecnologia

- **HTML5 + CSS3 + JavaScript vanilla** en un solo archivo.
- Tipografias: [Inter](https://fonts.google.com/specimen/Inter) y [Lora](https://fonts.google.com/specimen/Lora) (Google Fonts).
- Sin frameworks, sin build tools, sin backend.
- Compatible con cualquier navegador moderno (Chrome, Firefox, Safari, Edge).

---

## Licencia

MIT — Uso interno hospitalario. Contenido clinico basado en protocolos del servicio de COT.
