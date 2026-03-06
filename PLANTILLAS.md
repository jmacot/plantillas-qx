# Plantillas Quirúrgicas COT — Referencia Completa

> Catálogo de todas las plantillas del proyecto `plantillas-qx`,
> organizadas por región/categoría (quirófano) y módulo de urgencias.

> **Total: 90 plantillas quirúrgicas + 7 plantillas de urgencias = 97 plantillas** en 14 categorías quirúrgicas, 5 regiones anatómicas y 1 módulo de urgencias.

> **Variables dinámicas (quirófano):** `${FECHA}` (fecha DD/MM/YY), `${DOCTOR}` (cirujano), `${AYUDANTE}` (ayudante). **Lateralidad:** `${LADO_M}` (derecho/izquierdo), `${LADO_F}` (derecha/izquierda), `${LADO_M_UPPER}` (DERECHO/IZQUIERDO), `${LADO_F_UPPER}` (DERECHA/IZQUIERDA), `${LADO_ABR_F}` (DERECHA/IZQUIERDA), `${LADO_ABR_M}` (DERECHO/IZQUIERDO), `${DECUBITO}` (decúbito lateral contrario, minúscula), `${DECUBITO_UPPER}` (DECÚBITO LATERAL contrario, mayúscula).

> **Variables dinámicas (urgencias):** `${COT}` (nombre del COT de guardia), `${ACUDO}` (fórmula "Acudo/Acudimos"), `${PARTE}` (fórmula "como parte/por orden"), `${SEXO}` (Varón/Mujer), `${EDAD}` (edad del paciente), `${LADO}` (D/I para lateralidad).

---

## Índice

- [Trauma](#región-trauma)
  - [Trauma (18)](#categoría-trauma)
- [Rodilla](#región-rodilla)
  - [Artroscopia Rodilla (17)](#categoría-car)
  - [Prótesis Rodilla (3)](#categoría-ptr)
  - [LCA (12)](#categoría-lca)
  - [Osteotomías y Cartílago (8)](#categoría-rodilla_osteo)
- [Cadera](#región-cadera)
  - [Prótesis Cadera (3)](#categoría-ptc)
  - [Artroscopia Cadera (1)](#categoría-cac)
  - [Infiltración Cadera (1)](#categoría-ifc)
- [Miembro Superior](#región-ms)
  - [Artroscopia Hombro (4)](#categoría-hombro_mr)
  - [Prótesis Hombro (4)](#categoría-hombro_pthi)
  - [Tumores / Partes Blandas (1)](#categoría-hombro_tumor)
  - [Codo (3)](#categoría-codo)
  - [Mano y Antebrazo (10)](#categoría-ms)
- [Pie y Tobillo](#región-pt)
  - [Pie y Tobillo (5)](#categoría-pt)
- [Urgencias](#módulo-urgencias)
  - [Urgencias (7)](#categoría-urgencias)
- [Reglas Generales](#reglas-generales)

---

## Catálogo de Plantillas

<a id="región-trauma"></a>

### Región: Trauma

<a id="categoría-trauma"></a>

#### Trauma (18 plantillas)

##### `canulados_cadera` — Canulados cadera — tornillos canulados (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia: Regional.
- Profilaxis antibiótica: 2g de cefazolina intravenosa.
- Posición: Decúbito supino en mesa de tracción con control por escopia.
- Técnica quirúrgica: Reducción cerrada de la fractura de cadera ${LADO_F}.
- Fijación interna: Tres tornillos canulados en disposición de triángulo invertido:
- Tornillo inferior: 100 mm con arandela.
- Tornillos anterosuperior y posterosuperior: 100 mm y 95 mm respectivamente, sin arandela.
- Verificación: Comprobación de adecuada reducción y correcta colocación del material de osteosíntesis.
- Lavado: Abundante con suero fisiológico.
- Cierre: Por planos con sutura reabsorbible y piel con grapas.
- Apósito: Compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pie elevado cuando esté sentada, moviendo el pie según las indicaciones.
- Realizar ejercicios de rehabilitación tal como se le ha explicado.
- Vigilar coloración y sensibilidad del pie y los dedos.
- Evitar carga de peso sobre la pierna intervenida hasta nuevo aviso. Puede solicitar silla de ruedas en préstamo.
- Requiere ayuda domiciliaria para facilitar la movilidad y realizar las actividades diarias.

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575 mg cada 8 horas vía oral, alternando con PARACETAMOL 1g/8h si es necesario para el control del dolor.
- OMEPRAZOL 20 mg cada 24 horas.
- ENOXAPARINA 40 mg cada 24 horas vía subcutánea.
- VITAMINA D3: 4.000-6.000 UI/día durante 8-12 semanas, seguido de 2.000 UI/día de mantenimiento.
- Adecuada ingesta de calcio y proteínas en la dieta.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 48-72 horas.
- Retiro de grapas en 15-20 días, salvo mejor criterio de enfermería.

REVISIÓN
- Solicitar cita para revisión en consultas externas (${DOCTOR}) en 2-3 semanas para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
Acuda a Urgencias si presenta alguno de los siguientes síntomas:
- Fiebre superior a 38ºC.
- Dolor intenso que no se alivia con la medicación prescrita.
- Mala evolución de la herida (enrojecimiento, inflamación, supuración).
- Alteraciones en la sensibilidad o coloración de la extremidad intervenida.
- Dolor en el pecho, dificultad para respirar, o hinchazón excesiva en las piernas (posibles signos de trombosis venosa profunda).

RECOMENDACIONES PARA LOS CUIDADORES EN EL HOGAR

Movilización segura:
- Ayudar al paciente a mantener la pierna elevada y evitar movimientos bruscos.
- Evitar que el paciente realice esfuerzos excesivos o cargue peso sobre la pierna operada.
- Utilizar una silla de ruedas para los traslados si es necesario.

Cuidado de la herida:
- Asegúrese de que el paciente siga las indicaciones para las curas locales (cada 48-72 horas).
- Verifique que la herida esté limpia y seca, sin signos de infección (enrojecimiento, supuración o calor).
- Retirar las grapas en el plazo indicado (15-20 días) si no hay complicaciones.

Vigilancia de síntomas:
- Controle si el paciente tiene fiebre, dolor persistente o dificultad respiratoria, ya que estos podrían ser signos de infección o complicaciones.
- Mantenga un registro de la medicación que el paciente debe tomar, asegurándose de que reciba los analgésicos y anticoagulantes según lo prescrito.

Estimulación de la movilidad:
- Anime al paciente a realizar los ejercicios de rehabilitación que se le han enseñado, siempre con ayuda si es necesario, para evitar la atrofia muscular y mejorar la circulación.
- Ayude con la movilización pasiva si el paciente tiene dificultades para hacerlo por sí mismo.

Prevención de complicaciones:
- Vigile signos de trombosis venosa profunda (dolor en la pierna, hinchazón, enrojecimiento, y calor) y ayude a que el paciente se mueva para mejorar la circulación.
- Asegúrese de que el paciente mantenga la pierna elevada siempre que sea posible para reducir la hinchazón.
```

##### `gamma3` — Clavo Gamma3 — Fr pertrocantérea cadera (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Fractura pertrocantérea fémur ${LADO_M}.
- Anestesia regional.
- Profilaxis antibiótica con 2g de cefazolina.
- Decúbito supino, en mesa de tracción y con control por escopia. Reducción cerrada.
- Fijación interna con clavo Gamma 3 (Stryker) 125º x 10mm x 170mm, tornillo cefálico 90mm, tornillo de bloqueo distal 40mm.
- Comprobamos adecuada reducción y colocación de material de osteosíntesis.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con grapas.
- Apósito compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pie elevado cuando esté sentada, moviendo el pie como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar coloración y sensibilidad del pie y los dedos.
- Puede caminar con ayuda de andador, que solicitará en préstamo si precisa.
- Evitar cargar peso sobre pierna intervenida hasta nuevo aviso, puede solicitar silla de ruedas en préstamo.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas.
- ENOXAPARINA 40mg cada 24 horas vía subcutánea.
- DEMILOS 600mg/2000 UI 1 comprimido al día

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-20 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ptc_exeter` — PPC Exeter (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Fractura subcapital fémur ${LADO_M}
- Anestesia regional.
- Profilaxis antibiótica con 2g de cefazolina.
- Decúbito lateral ${DECUBITO}.
- Incisión longitudinal sobre región trocantérica y vía de abordaje según Bauer.
- Capsulotomía en “T” y osteotomía de cuello femoral. Resección de cabeza femoral.
- Artroplastia parcial de cadera cementada modelo Exeter (Stryker) vástago nº 35.5, cuello 0x26mm, cúpula bipolar 43mm.
- Comprobamos estabilidad en todos los planos.
- Sutura capsular y cierre por planos.
- Piel con grapas.
- Apósito compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pie elevado cuando esté sentada, moviendo el pie como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar coloración y sensibilidad del pie y los dedos.
- Puede caminar con ayuda de andador, que solicitará en préstamo si precisa.
- Requiere ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas.
- ENOXAPARINA 40mg cada 24 horas vía subcutánea.
- DELTIUS 10.000UI/ML 1 FRASCO 10ML 4 GOTAS cada 24 horas vía oral.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-20 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en un mes, para control evolutivo y radiológico (ACUDIR MEDIA HORA ANTES DE CITA PARA REALIZAR RX)

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `rafi_periprotesica` — RAFI Fr periprotésica cadera — Placa NCB (Zimmer)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

Fractura periprotésica de fémur ${LADO_M} en paciente con prótesis cadera
- Profilaxis antibiótica con 2 gr de cefazolina.
- Decúbito supino.
- Incisión longitudinal lateral del fémur.
- Vía abordaje subvasto externo e identificación de la fractura.
- Reducción abierta que se reduce con pinzas de reducción.
- Osteosíntesis con 2 tornillos interfragmentarios y placa periprotésica de fémur proximal NCB con 5 tornillos distales de 5 mm y 3 proximales de 4 mm + 3 cables ready.
- Se comprueba bajo escopia reducción fractura y longitudes de tornillos.
- Lavado abundante con suero.
- Cierre por planos.
- Drenaje aspirativo.
- Piel con grapas.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Reposo relativo SIN APOYO de la pierna intervenida.
- Puede requerir ayuda domiciliaria
- Movilización en silla de ruedas que se entregará a préstamo

MEDICACIÓN (según tarjeta sanitaria)
- PARACETAMOL 1 gr cada 8 horas alternando con METAMIZOL 575 mg cada 8 horas si dolor
- OMEPRAZOL 20 mg cada 24 horas vía oral
- ENOXAPARINA 40 mg cada 24 horas vía subcutánea
- DEMILOS 600 mg / 1000 UI 1 comprimido cada 24 horas

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `rafi_supracondilea` — RAFI Fr supracondílea fémur — Placa AXSOS (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

Fractura supraintercondílea de fémur ${LADO_M}
- Profilaxis antibiótica con 2 gr de cefazolina.
- Decúbito supino.
- Incisión longitudinal lateral del tercio distal del fémur.
- Vía abordaje subvasto externo e identificación de la fractura.
- Reducción de la fractura intercondílea y osteosíntesis con un tornillo intercondíleo de grandes fragmentos.
- RAFI con placa Axsos de titanio, tornillos distales looking y proximales.
- Se comprueba bajo escopia reducción fractura y longitudes de tornillos.
- Lavado abundante con suero.
- Cierre por planos.
- Piel con grapas.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Reposo relativo SIN APOYO de la pierna intervenida.
- Puede requerir ayuda domiciliaria
- Movilización en silla de ruedas que se entregará a préstamo

MEDICACIÓN (según tarjeta sanitaria)
- PARACETAMOL 1 gr cada 8 horas alternando con METAMIZOL 575 mg cada 8 horas si dolor
- OMEPRAZOL 20 mg cada 24 horas vía oral
- ENOXAPARINA 40 mg cada 24 horas vía subcutánea
- DEMILOS 600 mg / 1000 UI 1 comprimido cada 24 horas

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `rafi_rotula_cerclaje` — RAFI Fr rótula — cerclaje obenque (agujas K + alambre)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

Fractura transversal rótula ${LADO_F}
- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo.
- Incisión longitudinal anterior de rodilla.
- Identificación de fractura y osteosíntesis en obenque mediante 2 agujas de Kirschner paralelas y cerclaje de alambre en ocho.
- Se palpa congruencia articular a través de minificat.
- Lavado abundante con SF.
- Cierre por planos.
- Drenaje aspirativo intrarticular.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Reposo relativo SIN APOYO de la pierna intervenida.
- Puede requerir ayuda domiciliaria
- Movilización en silla de ruedas que se entregará a préstamo

MEDICACIÓN (según tarjeta sanitaria)
- PARACETAMOL 1 gr cada 8 horas alternando con METAMIZOL 575 mg cada 8 horas si dolor
- OMEPRAZOL 20 mg cada 24 horas vía oral
- ENOXAPARINA 40 mg cada 24 horas vía subcutánea
- DEMILOS 600 mg / 1000 UI 1 comprimido cada 24 horas

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `clavo_tibia_t2_stryker` — Clavo T2 tibia — fresado (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Fractura diafisaria multifragmentaria tibia ${LADO_F}.
- Anestesia regional.
- Profilaxis antibiótica con 2g de cefazolina.
- Decúbito supino, en mesa de tracción de tibia y con control por escopia.
- Reducción cerrada, abordaje transrotuliano y fresado progresivo.
- Tornillos interfragmentarios (26mm y 38mm).
- Osteosíntesis con clavo intramedular fresado T2 de 330x9 mm. Bloqueo proximal estático con tornillo de 40 mm. Bloqueo distal con 2 tornillos medio-lateral de 40 y 45 mm. Se coloca tapón en extremo proximal del clavo.
- Comprobamos adecuada reducción y colocación de material de osteosíntesis.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con grapas.
- Vendaje.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pie elevado cuando esté sentado, moviendo el pie como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado, haciendo flexión-extensión activa-asistida de rodilla frecuentemente.
- Vigilar coloración y sensibilidad del pie y los dedos.
- Evitar cargar peso sobre pierna intervenida hasta nuevo aviso y según plazos marcados, puede solicitar silla de ruedas en préstamo.
- Puede caminar con ayuda de muletas con carga parcial progresiva según le ha explicado su médico, que podrá solicitar en préstamo si precisa.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- NAPROXENO 500 / ESOMEPRAZOL 20 mg cada 12 horas vía oral añadido a lo anterior si precisa por dolor.
- ENOXAPARINA 40 mg cada 24 horas vía subcutánea.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-20 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de heridas, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `rafi_tobillo` — RAFI Tobillo — placa baja energía peroné distal (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Fractura transindesmal peroné ${LADO_M}.
- Anestesia raquídea.
- Profilaxis antibiótica con 2g de cefazolina.
- Isquemia profiláctica sobre miembro inferior ${LADO_M}.
- En decúbito supino y con control por escopia.
- Abordaje longitudinal sobre peroné distal, reducción abierta y fijación con tornillo interfragmentario.
- Fijación interna con placa baja energía 5 orificios, tornillos bloqueados distales y a compresión proximales.
- Comprobamos adecuada reducción y colocación de material de osteosíntesis.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con grapas.
- Apósito y férula suropédica.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pie elevado el mayor tiempo posible, moviendo dedos como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar coloración y sensibilidad de los dedos.
- Descarga de pie intervenido hasta nuevo aviso en consultas.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- ENOXAPARINA 40 mg cada 24 horas vía subcutánea.
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- OMEPRAZOL 20 mg cada 24h vía oral
- Vit D3 2000UI cada 24h vo

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `aquiles` — Sutura tendón Aquiles (mini-open, Ma-Griffith)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Intervenido por el ${DOCTOR}
- Tipo de anestesia: Raquídea
- Antibiótico profiláctico: Cefazolina 2 g IV
- Procedimiento:
- Abordaje mini-open
- Sutura según técnica de Ma-Griffith con hilo PDS 1
- Isquemia profiláctica en pierna ${LADO_F}
- Cierre por planos
- Inmovilización con férula anterior en equino
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS

Tratamiento pautado
- Puede requerir ayuda domiciliaria
- Paracetamol 1 g cada 8 horas
- Metamizol 575 mg cada 8 horas si hay dolor, alternando con el paracetamol
- Dexketoprofeno 25 mg cada 12 horas si el dolor no se controla
- Omeprazol 20 mg cada 24 horas
- Enoxaparina 40 mg una vez al día por vía subcutánea

Cuidados generales
- Mantenga el pie elevado y mueva los dedos con frecuencia.
- No apoyar el pie intervenido bajo ningún concepto.
- No mojar la férula ni introducir ningún objeto en su interior.
- No retire la férula hasta nueva indicación.

Protocolo de movilidad
- Semana 1: Férula anterior. Sin carga.
- Semana 2: Colocación de ortesis a -30º de flexión dorsal. Sin carga.
- Semana 3: Ortesis a -20º. Iniciar flexo-extensión activa en descarga, 3-4 veces al día, máximo 1 hora diaria.
- Semana 4: Ortesis a -10º. Puede retirarse la ortesis para dormir.
- Semana 5: Ortesis a 0º. Iniciar ejercicios de flexo-extensión activa contra resistencia, en descarga.
- Semana 6: Retirada definitiva de la ortesis. Iniciar carga parcial según tolerancia.

Síntomas de alarma
- Acuda a urgencias si presenta:
- Fiebre mayor a 38 ºC
- Enrojecimiento, inflamación o supuración abundante en la herida (No tomar antibióticos por cuenta propia)
- Dolor intenso no controlado con medicación
- Falta de aire, dolor en el pecho o hinchazón excesiva en las piernas

Revisión en consultas externas
- Solicitar cita con el ${DOCTOR} en 4 semanas.

Curas
- Solicite cita en sala de curas dentro de una semana.
- No realizar curas en casa hasta entonces.
- Evite fumar. El tabaco reduce el aporte de oxígeno a los tejidos y dificulta la cicatrización, especialmente en zonas con vascularización limitada como la parte medial del tendón de Aquiles. Esta región es especialmente sensible a complicaciones por su menor irrigación sanguínea, lo que aumenta el riesgo de retraso en la consolidación, dehiscencia de la herida e incluso fallo en la reparación tendinosa.
- Si necesita ayuda para dejar de fumar, consulte con su médico o farmacéutico.
```

##### `rafi_edr_aculoc2` — RAFI Fr distal radio — Placa Aculoc-2 (Acumed)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Bajo anestesia local y sedación, en decúbito supino, con manguito de isquemia en raíz de MSD, y con control por escopia.
- Abordaje de Henry sobre radio distal.
- Localización de fractura, reducción abierta y fijación interna con placa Aculoc-2 (Acumed).
- Lavado, hemostasia y cierre.
- Férula antebraquial.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la mano elevada, con el brazo en cabestrillo. Puede retirarlo cuando esté sentado y con la mano apoyada. Evitar declive.
- Mover activamente los dedos de la extremidad operada, según se le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- Si no control del dolor añadir DEXKETOPROFENO 25 mg cada 8 horas
- OMEPRAZOL 20mg cada 24 horas mientras precise medicación analgésica de forma continuada.
- VITAMINA C 500 mg cada 24 horas vía oral

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 48-72 horas, retirando puntos de sutura en 12-15 días, salvo mejor criterio de enfermería de zona.
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `rafi_humero_axsos` — RAFI Húmero proximal/diafisario — Placa AxSOS (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Fractura extremo proximal / diafisaria húmero ${LADO_M}.
- Anestesia general e IOT.
- Profilaxis antibiótica con 2g de cefazolina.
- En posición de silla de playa y con control por escopia.
- Abordaje deltopectoral ampliado a distal, reducción abierta.
- Tornillos interfragmentarios (24mm, 24mm y 26mm).
- Fijación interna con placa AxSOS (Stryker) 14 orificios.
- Comprobamos adecuada reducción y colocación de material de osteosíntesis.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con grapas.
- Apósito y cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener brazo en cabestrillo, moviendo mano y codo como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar coloración y sensibilidad de la mano y los dedos.
- Evitar cargar peso sobre brazo intervenido hasta nuevo aviso y según plazos marcados.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- NAPROXENO 500/ ESOMEPRAZOL 20 mg cada 12 horas vía oral añadido a lo anterior si precisa por dolor.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `rafi_clavicula` — RAFI Clavícula — Placa Variax (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Fractura diafisaria desplazada y con acortamiento clavícula ${LADO_F}.
- Anestesia general e IOT.
- Profilaxis antibiótica con 2g de cefazolina.
- En posición de silla de playa y con control por escopia.
- Abordaje directo sobre trazo, longitudinal a clavícula, reducción abierta.
- Tornillos interfragmentarios (24mm, 24mm y 26mm).
- Fijación interna con placa Variax (Stryker) 7 orificios. 6 tornillos no bloqueados 6x14mm.
- Comprobamos adecuada reducción y colocación de material de osteosíntesis.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con grapas.
- Apósito y cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener brazo en cabestrillo sobre ropa, moviendo mano y codo como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar coloración y sensibilidad de la mano y los dedos.
- Evitar cargar peso sobre brazo intervenido hasta nuevo aviso y según plazos marcados.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- NAPROXENO 500 / ESOMEPRAZOL 20 mg cada 12 horas vía oral añadido a lo anterior si precisa por dolor.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 48-72 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 3-4 semanas, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `monteggia` — Fr Monteggia / olécranon — Placa Peri-Loc (S&N)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Fractura luxación Monteggia codo ${LADO_M}.
- Anestesia regional.
- Profilaxis antibiótica con 2g de cefazolina.
- En decúbito supino y con control por escopia.
- Abordaje directo sobre cresta cubital y olécranon, reducción abierta.
- Tornillo interfragmentario (26mm).
- Fijación interna con placa Peri-Loc (Smith & Nephew) 7 orificios. 2 tornillos no bloqueados, 2 tornillos bloqueados. 2 bloqueados longitudinal.
- Comprobamos adecuada reducción y colocación de material de osteosíntesis.
- Cabeza radial reducida, no bloqueo en pronosupinación ni flexoextensión.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con grapas.
- Apósito y cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el brazo en cabestrillo, retirarlo cuando esté en reposo con brazo apoyado.
- Mover activamente los dedos de la extremidad operada, según se le ha explicado.
- Realizar frecuentemente ejercicios de pronosupinación y flexoextensión, según se le ha explicado y tolerancia.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral durante 5 días, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas durante 5 días.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 48-72 horas, retirando puntos de sutura en 15-18 días, salvo mejor criterio de enfermería de zona.
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma.
- Evitar coger peso y hacer fuerza con el brazo intervenido hasta nuevo aviso.

REVISIÓN
- Solicitar cita para revisión en CCEE COT ${DOCTOR} en 2-3 semanas, para control evolutivo.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, mala evolución de la herida, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_fr_radio` — Fr radio diafisario — placa

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo.
- Vía abordaje de Henry en cara anterior antebrazo.
- Se identifica fractura conminuta de 4 fragmentos.
- Reducción abierta y osteosíntesis con placa DCP-LC de 8 orificios (4 tornillos proximales y 3 distales).
- Cierre de TCS y piel con grapas.
- Se libera isquemia y coagula vasos sangrantes.
- Férula braquial.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el brazo  elevado  en cabestrillo
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- NOLOTIL 1 cápsula / 8 horas vía oral.
- OMEPRAZOL 20 mg/ 24  horas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (${DOCTOR}) en 3-4 semanas para Rx, valoración y seguimiento.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias. Mover activamente los dedos de la extremidad operada.
```

##### `ms_fr_cubito_radio` — Fr cúbito + radio — doble placa

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo.
- Vía abordaje de Henry en cara anterior antebrazo: RAFI con placa DCP-LC de 8 orificios.
- Vía abordaje dorsal sobre fractura de cúbito: RAFI con placa DCP-LC de 8 orificios (4 tornillos proximales y 3 distales).
- Se comprueba con escopia reducción de las fracturas y longitudes de tornillos.
- Lavado con suero fisiológico.
- Se libera isquemia y coagula vasos sangrantes.
- Cierre de TCS y piel con grapas.
- Férula braquial.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el brazo  elevado  en cabestrillo
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- NOLOTIL 1 cápsula / 8 horas vía oral,  alternar cada  4  horas  con PARACETAMOL 1 gr/8h si  dolor intenso.
- Revisión  en  CC EE de COT (${DOCTOR}) en 3 semanas aprox.  para Rx, valoración y  seguimiento.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias. Mover activamente los dedos de la extremidad operada.
```

##### `ms_fr_humero` — Fr húmero diafisario — placa

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- No se realiza isquemia.
- Incisión línea media posterior con vía de abordaje transtricipital.
- Se identifica fractura con tercer fragmento y se realiza limpieza foco.
- Reducción abierta y osteosíntesis con dos tornillos interfragmentarios solidarizando los dos fragmentos más distales y luego placa de neutralización DCP-LC de 12 orificios con 11 tornillos (5 proximales y 6 distales).
- Lavado abundante.
- Cierre por planos y piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el brazo  elevado  en cabestrillo
- Mover activamente los dedos de la extremidad operada  y  flexoextensión  del  codo
- Realizar los ejercicios que su médico le ha explicado.
- Prohibido hacer   ejercicios de   rotación  del  brazo, coger peso  y  realizar   actividades   de riesgo.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- METAMIZOL  575 mg / 8 horas vía oral.
- IBUPROFENO  600 mg/8  horas  via  oral  alterno  con  anterior   si  dolor  intenso
- OMEPRAZOL 20 mg/ 24  horas.
- Revisión  en  CC EE de COT (${DOCTOR}) en  3   semanas para Rx, valoración y  seguimiento.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_fr_olecranon_placa` — Fr olécranon — placa

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo.
- Vía abordaje posterior de codo.
- Se identifica fractura conminuta y se realiza limpieza foco.
- Reducción abierta y osteosíntesis con placa de olecranon preformada Peri-Loc de 8 orificios.
- Lavado abundante.
- Cierre de TCS y piel con grapas.
- Se libera isquemia.
- Férula braquial.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el brazo  elevado  en cabestrillo
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- METAMIZOL  575 mg / 8 horas vía oral.
- IBUPROFENO  600 mg/8  horas  via  oral  alterno  con  anterior   si  dolor  intenso
- OMEPRAZOL 20 mg/ 24  horas.
- Revisión  en  CC EE de COT (${DOCTOR}) en  3   semanas para Rx, valoración y  seguimiento.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias. Mover activamente los dedos de la extremidad operada.
```

##### `ms_fr_olecranon_cerclaje` — Fr olécranon — cerclaje

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo.
- Vía abordaje posterior de codo.
- Se identifica fractura y se realiza limpieza foco.
- Reducción abierta y osteosíntesis con 2 agujas de Kirschner del n.º 2 y cerclaje en obenque con alambre del 1.
- Se comprueba con escopia la correcta reducción de la fractura y colocación de las agujas.
- Lavado abundante.
- Cierre por planos y piel con grapas.
- Se libera isquemia.
- Férula braquial.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el brazo  elevado  en cabestrillo
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- METAMIZOL 575 mg / 8 horas vía oral.
- IBUPROFENO  600 mg/8  horas  via  oral  alterno  con  anterior cada  4  horas,  si  dolor  intenso
- OMEPRAZOL 20 mg/ 24  horas.
- Revisión  en  CC EE de COT (${DOCTOR}) en  2 semanas para Rx, cura herida qca y  seguimiento.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias. Mover activamente los dedos de la extremidad operada.
```

<a id="región-rodilla"></a>

### Región: Rodilla

<a id="categoría-car"></a>

#### Artroscopia Rodilla (17 plantillas)

##### `car_mosaicoplastia` — CAR Mosaicoplastia

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Portales accesorios anteromedial para zona receptora y parapatelar medial para zona donante.
- Articulación femoropatelar y fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: lesión osteocondral grado 3 inestable en zona lateral del cóndilo femoral interno de aproximadamente 2 cm diámetro. Desbridamiento de la misma con sinoviotomo, fresa esférica y regularización de los bordes con cucharilla.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Toma de 2 injertos osteocondrales de 8.5 mm diámetro en zona medial de troclea femoral y 1 injerto de 6.5 mm en zona lateral, todos de unos 17-18 mm longitud.
- Perforación de 3 túneles correspondientes en zona receptora de unos 18-20 mm y colocación de los 3 injertos osteocondrales según técnica habitual de mosaicoplastia.
- Cierre portales con grapas.
- Drenaje aspirativo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  SIN  APOYO de  la pierna intervenida  hasta  nueva orden  (aproximadamente 6  semanas).
- Realizar ejercicios isométricos de cuádriceps y  movilidad libre de  la rodilla en  descarga.
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA  40 mg /24 horas vía subcutánea
- Retirada de puntos por ATS DE ZONA en 12/15 días.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3 semanas  para ver evolución.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_fr_meseta` — CAR + Fr meseta tibial

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin lesiones meniscales ni condrales.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: no lesiones meniscales. Fractura de borde lateral de meseta tibial con hundimiento y separación.
- Lavado articular abundante.
- Se identifica fractura, con guía de LCA se realiza perforación de cortical medial de tibia y se asciende fragmento fracturado con impactador.
- Osteosíntesis con 2 tornillos percutáneos de esponjosa rosca parcial larga de 6.5 *60 mm con arandelas mediante control de escopia.
- Se rellena túnel tibial con Prosteon taco y gránulos.
- Cierre portales.
- Drenaje aspirativo.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  SIN APOYO  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y  movilidad limitada de la rodilla 0º-60º hasta nueva orden
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- PARACETAMOL 1 g / 8 horas (alterno con anterior cada 4 horas, si dolor intenso)
- ENOXAPARINA  40 mg/24 horas - vía subcutánea
- Retirada de puntos por ATS DE ZONA en 12/15 días.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3/4 semanas  para ver evolución.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_reinsercion_espina` — CAR Reinserción avulsión espina tibial LCA

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral. Portal medial accesorio.
- Articulación femoropatelar y fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno y ext: sin lesiones meniscales ni hundimiento de meseta tibiales.
- Pivote central: avulsión de espina tibial a nivel de la inserción del LCA con éste íntegro. LCP íntegro y competente.
- Lavado articular abundante.
- Se identifica fractura, se limpia lecho óseo y se retira ligamento intermeniscal que impedía la reducción de la avulsión.
- Se pasa doble sutura en marco en la base del LCA. Ambas se pasan por dos minitúneles desde el lecho de fractura y se anudan en la cortical anterior de tibia dejando un puente óseo de algo más de 1 cm.
- Se comprueba con escopia reducción fragmento y tensión del LCA.
- Cierre portales.
- Drenaje aspirativo.
- Inmovilización con ortesis en extensión.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  SIN APOYO  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps e  isquiotibiales.
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- METAMIZOL 575  mg   /  8 horas (alterno  con anterior cada 4  horas,  si  dolor intenso)
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA  40 mg/24 horas - vía subcutánea
- Retirada de puntos por ATS DE ZONA en 12/15 días.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3 semanas  para ver evolución(Forzar si  es preciso!!!)

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.

Postoperatorio:
- 0-2 semanas:
- Rodillera   bloqueada en  extensión  y  descarga.
- Isométricos de   cuádriceps e  isquiotibiales.
- EPE.
- Movilizaciones de la patela.
- 2-4 semanas:
- Carga  progresiva con  rodilla en  extensión ayudado  por  muletas.
- Retirada   de la inmovilización  y  comiezo  de protocolo de  RHB  para conseguir   rango  de  movilidad  0-90º
- 6ª semana:
- Ejercicios   activos de movilidad.
- Se retiran  las  muletas.
- 8ª semana:
- Movilidad activa  y  pasiva completos.
- Bicicleta estática  y  natación.
- 16ª  semana:
- Running  y  retorno  a actividades deportivas.
```

##### `car_lrr_ficat_plicatura` — CAR Ficat + plicatura ARI (Lanny Johnson)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- No se aprecia lesiones meniscales ni ligamentosas.
- Articulación femoropatelar y fondos de saco cuadricipitales: subluxación lateral de rótula con condropatía grado 3.
- Se realiza sección alerón rotuliano externo artroscópico (Ficat) con vaporizador.
- Plicatura de alerón rotuliano interno por técnica artroscópica de Lanny Johnson con 3 puntos de sutura con Safil del nº 2.
- Se comprueba buen tracking rotuliano posteriormente a realineación.
- Lavado articular abundante.
- Cierre portales con seda.
- Drenaje aspirativo.
- Férula inguinomaleolar.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Aplicar hielo sobre la rodilla operada 2-3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda bastones con apoyo de la pierna intervenida.
- Puede requerir ayuda domiciliaria
- NOLOTIL 1 cápsula / 8 horas vía oral.
- Si  dolor  intenso  alternar cada  4  horas con  IBUPROFENO  600 mg/ 8  horas
- PARACETAMOL 1 gr cada 8 horas
- OMEPRAZOL 20 mg/ 24 horas.
- BEMIPARINA  3500 UI / 24 horas vía subcutánea / 3 semanas.
- Revisión en CC EE de COT (${DOCTOR}) en  2/3 semanas para retirar férula y seguimiento.
- Al  alta  solicitar cita en  SERVICIO  DE  REHABILITACIÓN  para inicio  de fisioterapia tras retirada de   férula  de yeso

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias. Mover activamente los dedos de la extremidad operada.
```

##### `car_sher_plicatura` — CAR SHER plicatura ARI + Ficat

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Portal superoexterno accesorio.
- Articulación femoropatelar y fondos de saco cuadricipitales: subluxación rotuliana externa sin condropatía.
- Compartimento interno: sin alteraciones.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: rotura radial del cuerpo del ME que se regulariza con pinzas y motor.
- Realineamiento proximal rotuliano mediante técnica artroscópica modificada de Halbrecht: plicatura del alerón rotuliano int con 4 puntos de sutura all inside con PDS del nº 1.
- Se comprueba buen tracking rotuliano posteriormente a realineación.
- No precisa Ficat.
- Lavado articular abundante.
- Cierre portales con seda.
- Drenaje aspirativo.
- Férula inguinomaleolar.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Aplicar hielo sobre la rodilla operada 2-3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda bastones con apoyo parcial de la pierna intervenida.
- Ejercicios  isométricos de cuádriceps y de elevación  con  pierna   extendida  (EPE) aproximadamente  unas  15-20 veces cada  hora.
- Mantener   la ortesis   bloqueada  en  extensión completa  durante   primera semana.

Movilidad  progresiva   a  razón  de  :
- 2º semana: BA de  0º  a 30º.
- 3º y  4º semanas:  BA de  0º a 60º.
- 5º  y  6º semanas:  BA  de  0º a  90º. (No  está  permitido  flexionar   más de  90º  en  las  primeras  4  semanas).
- A partir de las   6 semanas  movilidad  libre sin ortesis.
- Reincorporación  a  la actividad deportiva  de forma progresiva comenzando  con carrera suave a partir de los 3 meses.
- Deportes de impacto  con   cambios de ritmo  y  dirección  más bruscos   entre  los 4  y  6  meses.
- Puede requerir ayuda domiciliaria
- METAMIZOL 575 mg / 8 horas vía oral.
- Si  dolor  intenso  alternar cada  4  horas con  IBUPROFENO  600 mg/ 8  horas.
- PARACETAMOL 1 gr cada 8 horas
- OMEPRAZOL 20 mg/ 24 horas.
- BEMIPARINA  3500 UI / 24 horas vía subcutánea / 3 semanas.
- Revisión en CC EE de COT (${DOCTOR}) en  2/3 semanas para seguimiento.
- Al  alta  solicitar cita en  SERVICIO  DE  REHABILITACIÓN  para inicio  de fisioterapia tras retirada de   férula  de yeso

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias. Mover activamente los dedos de la extremidad operada.
```

##### `car_otv_adiccion` — CAR + OTV adicción

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER} + osteotomía de adicción valguizante de tibia ${LADO_F_UPPER}:
- Isquemia en muslo ${LADO_M}.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía de la tróclea femoral grado 4.
- Compartimento interno: rotura degenerativa del cuerpo y cuerno posterior del menisco interno que se reseca y regulariza con pinzas y motor. Condropatía grado 4 de toda zona carga de cóndilo femoral int y meseta tibial int.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Extracción de injerto bicortical de cresta iliaca y chips de esponjosa.
- Incisión oblicua en tercio proximal y medial de tibia siguiendo dirección de los tendones isquiotibiales.
- Desinserción parcial de la inserción distal del fascículo superficial del LLI.
- Osteotomía biplanar de tibia respetando la TTA con sierra y completada con escoplo.
- Apertura de la cuña de forma progresiva hasta 16º y relleno de la misma con el injerto autólogo cortical y de esponjosa.
- Osteosíntesis con placa de osteotomía tibial medial proximal Tomofix fijada con 4 tornillos proximales y 4 tornillos distales fijados a placa.
- Cierre por planos.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos,  tobillo y  rodilla  de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  SIN  APOYO  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y  movilidad libre de  la rodilla
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- METAMIZOL  1  cápsula/ 8 horas via oral  alterno  con  Ibuprofeno  cada  4  horas.
- PARACETAMOL 1 gr cada 8 horas
- OMEPRAZOL  20 mg/ 24  horas
- BEMIPARINA 3500 UI /24 horas vía subcutánea

Curas por  ATS DE  ZONA con  Betadine  cada  48/72 horas.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3 semanas  para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_otv_sustraccion` — CAR + OTV sustracción (Coventry)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER} + osteotomía de sustracción valguizante de tibia ${LADO_F_UPPER} tipo Coventry:
- Isquemia en muslo ${LADO_M}.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía tróclea femoral grado 4.
- Compartimento interno: rotura degenerativa del cuerpo y cuerno posterior del menisco interno que se reseca y regulariza con pinzas y motor. Condropatía grado III de toda zona carga de cóndilo femoral int y meseta tibial int.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Lavado articular abundante.
- Cierre portales con seda.
- Vendaje compresivo.
- Incisión en L desde TTA, borde lat tendón rotuliano e interlínea externa.
- Desinserción del tibial anterior y exposición metáfisis tibial.
- Despegamiento sindesmosis tibioperoneal.
- Osteotomía tibia y resección de cuña de sustracción de base lat de 9º.
- Cierre de la cuña mediante osteoclasia medial y osteosíntesis con placa de osteotomía tibial Nexgen de 8 mm offset fijada con 2 tornillos de esponjosa proximales de 65 y 60 mm y 2 de cortical de 4.5 mm de 44 y 54 mm.
- Reinserción músculo tibial anterior.
- Drenaje aspirativo.
- Cierre por planos.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos,  tobillo y  rodilla  de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  SIN  APOYO  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y  movilidad libre de  la rodilla
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- METAMIZOL  1  cápsula/ 8 horas via oral  alterno  con  Ibuprofeno  cada  4  horas.
- PARACETAMOL 1 gr cada 8 horas
- OMEPRAZOL  20 mg/ 24  horas
- ENOXAPARINA 60 mg /24 horas vía subcutánea

Curas por  ATS DE  ZONA con  Betadine  cada  48/72 horas.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3 semanas  para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_otv_varizante_femur` — CAR + Osteotomía varizante fémur

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER} + osteotomía supracondílea de sustracción varizante de fémur ${LADO_M}:
- No se realiza isquemia.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía grado 3 con resección protuberancia de partes blandas a nivel tróclea femoral.
- Compartimento interno: sin alteraciones de interés.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: rotura degenerativa del cuerpo y cuerno anterior del menisco ext que se reseca y regulariza con pinzas y motor. Condropatía grado 2/3 de cóndilo femoral ext.
- Lavado articular abundante.
- Cierre portales con grapas.
- Incisión anteromedial de tercio distal de fémur ${LADO_M} y abordaje subvasto int.
- Osteotomía supracondílea oblicua biplanar de sustracción de base interna de 12º.
- Cierre de la cuña mediante osteoclasia lateral progresiva y osteosíntesis con placa Tomofix de fémur distal medial ${LADO_M} con 4 tornillos epifisarios distales y 4 tornillos proximales todos con bloqueo en placa.
- Se comprueba con escopia cierre osteotomía y longitud y situación de los tornillos.
- Lavado herida quirúrgico abundante.
- Sutura de la fascia del vasto int.
- Drenaje aspirativo.
- Cierre por planos.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos,  tobillo y  rodilla  de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  SIN  APOYO  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y  movilidad libre de  la rodilla
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- METAMIZOL  1  cápsula/ 8 horas via oral  alterno  con  Ibuprofeno  cada  4  horas.
- PARACETAMOL 1 gr cada 8 horas
- OMEPRAZOL  20 mg/ 24  horas
- ENOXAPARINA 60 mg /24 horas vía subcutánea

Curas por  ATS DE  ZONA con  Betadine  cada  48/72 horas.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3 semanas  para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_otv_tomofix` — OTV placa Tomofix (sin CAR)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Osteotomía de adicción valguizante de tibia ${LADO_F_UPPER}:
- Isquemia en muslo ${LADO_M}.
- Incisión oblicua en tercio proximal y medial de tibia siguiendo dirección de los tendones isquiotibiales en su borde anterior.
- Desinserción parcial de la inserción distal del fascículo superficial del LLI.
- Osteotomía biplanar de tibia respetando la TTA con sierra y completada con escoplo.
- Apertura de la cuña de forma progresiva hasta 12º y relleno de la misma con injerto autólogo tricortical de cresta iliaca.
- Osteosíntesis con placa de osteotomía tibial medial proximal Tomofix fijada con 4 tornillos proximales y 4 tornillos distales fijados a placa.
- Cierre por planos.
- Drenaje aspirativo.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos,  tobillo y  rodilla  de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  SIN  APOYO  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y  movilidad libre de  la rodilla
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- PARACETAMOL  1 gra/ 8 horas via oral  alterno  con  Ibuprofeno  cada  4  horas.
- OMEPRAZOL  20 mg/ 24  horas
- CLEXANE 40 mg /24 horas vía subcutánea hasta deambulación  normal con carga completa.

Curas por  ATS DE  ZONA cada  48/72 horas.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3 semanas  para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_meniscectomia` — CAR Meniscectomía parcial

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: rotura degenerativa del cuerno posterior del menisco interno que se reseca y regulariza con pinzas y motor.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Lavado articular abundante.
- Se infiltra portales y región intraarticular con ropivacaína y ácido hialurónico.
- Cierre portales con seda.
- Vendaje compresivo.
- EVOLUCIÓN: Durante el postoperatorio el paciente se ha mantenido afebril y hemodinámicamente estable. Ha presentado buen control del dolor con la analgesia pautada, sin evidenciarse deficits vasculonerviosos ni signos de TVP en el miembro intervenido. Ha tolerado correctamente la sedestación y la deambulación asistida. La herida quirúrgica no ha presentado signos de complicación local.
- Dada la evolución favorable la paciente es alta a domicilio.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 3 - 4 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas con apoyo de la pierna intervenida
- Puede requerir ayuda domiciliaria

MEDICACION
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 10 días.

ANALGESIA BASAL:
- -PARACETAMOL 1 g/8h oral alterno con combinación de Dexketoprofeno 25 mg y Tramadol 75 mg (Enanplus) cada 8 horas oral durante 3 días.
- Mientras dure el tratamiento con AINE: Omeprazol 20 mg/24h oral
- -ANALGESIA DE RESCATE: Metamizol 575 mg/8h oral.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Antes de irse de alta  del  hospital  solicitar  en  Admisión  de  Consultas  revisión en CC EE  de  COT (${DOCTOR})  en   unas  3/4 semanas  para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.

EJERCICIOS POSTOPERATORIOS
- Objetivo: recuperar movilidad, fuerza y reincorporarse progresivamente a las actividades habituales sin dolor ni inflamación.

Indicaciones generales
- Puede apoyar la pierna operada desde el primer día según tolerancia.
- Utilice muletas si tiene dolor o cojea. Normalmente se retiran en 3-5 días.
- Puede mover la rodilla libremente desde el principio.
- No es necesario el uso de rodillera.

Ejercicios recomendados (2 veces al día, 10 repeticiones cada uno)
- Contracciones del cuádriceps (apretar el muslo contra la cama).
- Elevación de pierna recta (tumbado, elevar pierna estirada).
- Movilidad de rodilla: flexionar y extender en cama sin dolor.
- Puente glúteo (elevar la pelvis con ambos pies apoyados).
- Ejercicios de tobillo (movimientos arriba-abajo y circulares).

Evitar
- Saltos o carrera antes de las 4 semanas.
- Sentadillas profundas o escaleras si hay dolor.
- Deportes de impacto antes de la revisión médica.

Progresión esperada
- Caminar sin muletas: 5-10 días.
- Recuperar flexión completa: 2-3 semanas.
- Actividad física moderada: a partir de 4 semanas.
- Retorno al deporte: según evaluación clínica (aprox. 6 semanas).
```

##### `car_sutura_meniscal` — CAR Sutura meniscal

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: rotura en asa de cubo reducida en zona roja del cuerpo y cuerno posterior del menisco interno. Reducción y sutura con 4 puntos con sistema Fast-Fix y dos puntos sutura fuera dentro con Ticron 2.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Lavado articular abundante.
- Se infiltra portales y región intraarticular con ropivacaína + AH
- Cierre portales.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas SIN  APOYO  inicial de la pierna intervenida:
- Semana 0 – semana 3: descarga completa.
- Semana 3 – semana 6: carga parcial con ayuda de bastones.
- A partir  semana 6: puede caminar libremente sin  bastones (apoyo  completo).
- Aumento  progresivo  de la  movilidad para protección de la sutura meniscal:
- Semana 0 - semana 2: 0º a 60º.
- Semana 2 - semana 4:  0º  a 90º.
- Semana 4- semana 6: 90º a 120º.
- A partir  semana 6:  movilidad libre.
- Realizar ejercicios isométricos de cuádriceps y elevación con  pierna extendida.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria

MEDICACION:
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 10 días.

ANALGESIA BASAL:
- -PARACETAMOL 1 g/8h oral alterno con combinación de Dexketoprofeno 25 mg y Tramadol 75 mg (Enanplus) cada 8 horas oral durante 3 días.
- Mientras dure el tratamiento con AINE: Omeprazol 20 mg/24h oral
- Si náuseas: Ondansetrón 4 mg/8h oral
- -ANALGESIA DE RESCATE: Metamizol 575 mg/8h oral.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (${DOCTOR}) a  las  2 semanas  para ver evolución y ampliar  rango  de movilidad.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_artrolisis` — CAR Artrolisis + movilización bajo anestesia

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER} en paciente con rigidez postoperatoria tras artroplastia rodilla:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Se aprecia múltiples adherencias y fibrosis a nivel de fondos de saco subcuadricipitales y del Hoffa que se reseca con sinoviotomo.
- Coagulación de puntos sangrantes con vaporizador.
- No se aprecia alteraciones de la prótesis de rodilla.
- Tras artrolisis y movilización bajo anestesia se consigue un balance articular de 0-140º
- Lavado articular abundante.
- Cierre portales.
- Drenaje aspirativo.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 3 - 4 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas con apoyo de la pierna intervenida
- Realizar ejercicios isométricos de cuádriceps y movilidad libre de la rodilla.
- Puede requerir ayuda domiciliaria
- ENANPLUS 1   comp/ 8  h
- PARACETAMOL 1 gr cada 8 horas
- INHIXA 40 / 24 horas vía subcutánea durante  10  días

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (${DOCTOR}) en 3/4 semanas  para seguir  evolución.
- Continuar  con sesiones de Rehabilitación  para tratar de   mantener  la  movilidad (SOLICITAR CITA  ANTES DEL  ALTA)

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_diagnostica` — CAR Diagnóstica

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin alteraciones.
- Pivote central: LCA y LCP íntegros y competentes.
- Compartimento externo: sin alteraciones.
- Lavado articular abundante.
- Se infiltra portales y región intraarticular con ropivacaína y ácido hialurónico.
- Cierre portales con seda.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  con  apoyo  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y  movilidad libre de  la rodilla
- Puede requerir ayuda domiciliaria
- METAMIZOL  575 mg /8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- BEMIPARINA  3500 UI /24 horas vía subcutánea  durante 10 días.
- Retirada de puntos por ATS DE ZONA en 12/15 días.
- Revisión en CC EE  de  COT (${DOCTOR})  en unas  4-5   semanas  para ver evolución.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_cuerpo_libre` — CAR Extraccion cuerpo libre (no registrada en UI)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin alteraciones.
- Pivote central: LCA y LCP íntegros y competentes.
- Compartimento externo: sin alteraciones.
- Se localiza y extrae cuerpo libre intraarticular de aproximadamente 1 cm de diámetro en fondo de saco subcuadricipital.
- Lavado articular abundante.
- Se infiltra portales y región intraarticular con ropivacaína y ácido hialurónico.
- Cierre portales con seda.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas con apoyo de la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y movilidad libre de la rodilla.
- Puede requerir ayuda domiciliaria
- METAMIZOL 575 mg /8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- BEMIPARINA 3500 UI /24 horas vía subcutánea durante 10 días.
- Retirada de puntos por ATS DE ZONA en 12/15 días.
- Revisión en CC EE de COT (${DOCTOR}) en unas 4-5 semanas para ver evolución.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_ficat` — CAR Ficat

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: síndrome de hiperpresión rotuliana externa sin condropatía. Se realiza sección alerón rotuliano externo artroscópico (Ficat) con vaporizador.
- Compartimento interno: sin alteraciones.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Lavado articular abundante.
- Se infiltra portales y región intraarticular con bupivacaína 0.5 con VC.
- Cierre portales con seda.
- Drenaje aspirativo.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas  con  apoyo  de  la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y  movilidad libre de  la rodilla
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 15 días.
- Retirada de puntos por ATS DE ZONA en 12/15 días.
- Revisión en CC EE  de  COT (${DOCTOR})  en  3 semanas  para ver evolución.

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_toilette` — CAR Toilette

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER}:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía FP grado 4.
- Compartimento interno: rotura degenerativa del cuerpo y cuerno post del menisco int que se regulariza con pinzas y sinoviotomo. Condropatía CFI grado 4.
- Pivote central: LCA y LCP íntegros y competentes.
- Compartimento externo: rotura degenerativa del cuerpo y cuerno ant del menisco ext que se regulariza. Condropatía MTE grado 4 y CFE grado 3.
- Lavado articular y toilette general de la rodilla.
- Extracción de 3-4 cuerpos libres por condromatosis sinovial entre 0.5-1 cm diámetro.
- Se deja drenaje articular aspirativo.
- Cierre portales con seda.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 3 - 4 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas con apoyo de la pierna intervenida
- Realizar ejercicios isométricos de cuádriceps y movilidad libre de la rodilla
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral durante  una semana.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 10 días.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Antes de irse de alta  del  hospital  solicitar  en  Admisión  de  Consultas  revisión en CC EE  de  COT (${DOCTOR})  en   unas  3/4 semanas  para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `car_sinovectomia` — CAR Sinovectomía total

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- CAR ${LADO_F_UPPER} en paciente con derrame de repetición por sospecha de sinovitis villonodular pigmentada:
- Isquemia en raíz de muslo.
- Portales tradicionales anteromedial y anterolateral.
- Portal accesorio superolateral y superomedial.
- Se aprecia sinovial hiperémica e hipertrófica en toda la rodilla formando vellosidades y con tinción parduzca por hemartros de repetición.
- Se toma muestra de sinovial para anatomía patológica.
- Sinovectomía radical a través de todos los portales.
- No lesiones meniscales, condrales ni ligamentosas.
- Lavado articular abundante.
- Se infiltra portales y región intraarticular con ropivacaína + corticoides.
- Cierre portales con grapas.
- Drenaje aspirativo.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 3 - 4 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas con apoyo de la pierna intervenida
- Realizar ejercicios isométricos de cuádriceps y movilidad libre de la rodilla
- Puede requerir ayuda domiciliaria
- IBUPROFENO  600 mg / 8 horas vía oral.
- Alternar cada 4  horas con METAMIZOL 575 mg/8  horas si  dolor intenso
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA  40 mg  / 24 horas vía subcutánea.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (${DOCTOR}) en 3 semanas  para seguir  evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

<a id="categoría-ptr"></a>

#### Prótesis Rodilla (3 plantillas)

##### `ptr_triathlon` — PTR Triathlon (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Gonartrosis rodilla ${LADO_F}.
- Profilaxis antibiótica con 2g de Cefazolina.
- La intervención se realiza sin isquemia.
- Abordaje longitudinal anterior y artrotomía pararrotuliana medial.
- Prótesis total rodilla modelo Triathlon (STRYKER):
- Componente femoral CR no cementado nº 4.
- Componente tibial cementado nº 4.
- Inserto tibial CR 9mm.
- Patela:
- Se comprueba adecuado balance mediolateral en flexión y extensión, y adecuado tracking rotuliano.
- Cierre por planos.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la rodilla 3-4 veces al día durante 10-15 minutos.
- Mover activamente los dedos de la extremidad operada.
- Puede requerir ayuda domiciliaria

MEDICACION (incluida en su tarjeta sanitaria):
- METAMIZOL 1 cápsula / 8 horas vía oral.
- PARACETAMOL 1 g / 8 horas, alterno con anterior cada 4 horas si dolor intenso.
- TRAMADOL 50 mg cada 12 horas como rescate durante 10 días
- ENOXAPARINA 3500UI / 24 horas vía subcutánea durante 6 semanas.

Signos de alarma de infección
- Fiebre persistente (mayor de 38 °C)
- Escalofríos intensos
- Enrojecimiento, sensibilidad o hinchazón crecientes en la herida
- Secreción por la herida
Signos de alarma de trombosis venosa
- Dolor en la pierna o pantorrilla no relacionado con la incisión
- Sensibilidad o enrojecimiento por encima o por debajo de la rodilla
- Hinchazón creciente en pantorrilla, tobillo o pie
- En casos muy raros, un coágulo puede desplazarse al pulmón y ser potencialmente mortal. Signos de embolia pulmonar:
- Dificultad respiratoria
- Dolor torácico repentino
- Dolor localizado en el pecho al toser
- Informa a tu médico de inmediato si presentas alguno de estos síntomas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Con este informe solicitará cita en consultas del ${DOCTOR} en 4 semanas. La primera revisión se realizará sin Rx control salvo petición por su Doctor.
```

**Tratamiento al Alta — Ejercicios (opcional, toggle en UI):**

```
EJERCICIOS POSTOPERATORIOS

Encamado (primeros días tras intervención)

- Mover el tobillo:
  Objetivo: Facilitar el retorno venoso y reducir la inflamación.
  Cómo hacerlo: Acostado(a) en la cama, mueva ambos tobillos hacia arriba y hacia abajo repetidamente.
  Frecuencia: Realice el mayor número de veces posible durante el día.

- Contracción del cuádriceps:
  Objetivo: Fortalecer el músculo del muslo y mejorar la extensión de la rodilla.
  Cómo hacerlo: Coloque una toalla enrollada debajo de la rodilla. Contraiga el cuádriceps (músculo del muslo) intentando "aplastar" la toalla contra la cama.
  Duración: Mantenga la contracción durante 5 segundos.
  Repeticiones: Hágalo de 10 a 20 veces, 2-3 veces al día.

- Elevación de pierna recta:
  Objetivo: Fortalecer los músculos de la pierna operada.
  Cómo hacerlo: Con la pierna sana doblada, mantenga la pierna operada recta, elévela unos 20-30 cm de la cama, mantenga por 5 segundos y bájela lentamente.
  Repeticiones: Realice de 100 a 300 elevaciones a lo largo del día.

- Flexión de rodilla en cama:
  Objetivo: Mejorar el rango de movimiento de la rodilla.
  Cómo hacerlo: Deslice el talón de la pierna operada hacia los glúteos doblando la rodilla. Mantenga la flexión máxima por 5 segundos y luego vuelva a estirar la pierna.
  Repeticiones: Realice de 10 a 15 veces, 2-3 veces al día.

Ejercicios sentado(a) en silla

- Flexión de rodilla:
  Objetivo: Mejorar la flexión de la rodilla.
  Cómo hacerlo: Sentado(a) en el borde de una silla, con el pie en el suelo, flexione la rodilla operada lo máximo posible. Ayúdese con la pierna sana para aumentar la flexión. Mantenga la posición durante 5-10 segundos y luego estire la pierna.
  Repeticiones: Hágalo de 10 a 15 veces, 2-3 veces al día.

- Extensión de rodilla:
  Objetivo: Mejorar la extensión completa de la rodilla.
  Cómo hacerlo: Sentado(a) en el borde de la silla, estire la pierna operada lo máximo posible. Ayúdese con la pierna sana para lograr una extensión máxima. Mantenga la posición durante 5-10 segundos y luego vuelva a la posición inicial.
  Repeticiones: Realice de 10 a 15 veces, 2-3 veces al día.

- Extensión pasiva de rodilla:
  Objetivo: Mejorar la movilidad y reducir la rigidez.
  Cómo hacerlo: Coloque una silla frente a usted y extienda la pierna operada sobre ella, dejando que la rodilla se relaje y se extienda de forma pasiva durante 5-10 minutos.
  Frecuencia: Hágalo después de los ejercicios de flexión-extensión.

- Potenciación de aductores:
  Objetivo: Fortalecer los músculos aductores del muslo.
  Cómo hacerlo: Coloque un cojín entre los muslos y presione hacia el centro con ambas piernas.
  Duración: Mantenga la presión por 10 segundos.
  Repeticiones: Realice 10 veces, 2-3 veces al día.

CAMINAR CON MULETAS
- Primer paso: Avance las muletas.
- Segundo paso: Adelante la pierna operada hasta el nivel de las muletas.
- Tercer paso: Avance la pierna sana.

Uso de una sola muleta
- Cuando pase a usar una sola muleta, esta debe estar en el lado contrario a la pierna operada, avanzando a la vez que la pierna intervenida.

CAMINAR CON ANDADOR
- Coloque el andador frente a usted, con las cuatro patas firmemente apoyadas en el suelo. Ajústelo a su altura.
- Paso 1: Desplace el andador un paso hacia adelante (aproximadamente un brazo de distancia).
- Paso 2: Avance la pierna operada hacia el centro del andador, entre las patas delanteras.
- Paso 3: Avance la pierna sana hasta alcanzar la posición de la pierna operada.
- Repita el ciclo manteniendo el andador siempre delante de usted.

Consejos
- Mantenga una postura erguida para reducir el riesgo de caídas.
- Avance el andador siempre antes de dar el paso con la pierna operada.
- No se apresure. Camine a un ritmo que le permita sentirse seguro(a) y estable.

SUBIR Y BAJAR ESCALERAS

Para subir escaleras
- Coloque la pierna sana en el escalón superior.
- Apóyese en las muletas y la pierna sana para levantar la pierna operada.

Para bajar escaleras
- Coloque las muletas en el escalón inferior.
- Baje la pierna operada.
- Luego, baje la pierna sana.

CUIDADOS DE LA HERIDA
- Mantenga la herida limpia y seca. Cambie los apósitos según lo indicado por su médico.
- Evite mojar la herida. Utilice coberturas impermeables si se ducha.
- Observe signos de infección: enrojecimiento, calor, secreciones o aumento del dolor en la zona.
- NO FUMAR. El tabaco compromete la cicatrización, aumenta el riesgo de infección y retrasa la recuperación. Se recomienda evitarlo completamente durante el proceso de recuperación.
- Ante complicaciones en la herida: NO tomar antibióticos por cuenta propia. Acuda a urgencias para valoración médica.
```

##### `puc_pkr` — PUC PKR (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Genu varo artrósico rodilla ${LADO_F_UPPER}:
- Profilaxis antibiótica con 2 gr de CEFAZOLINA.
- Isquemia en raíz de muslo.
- Incisión longitudinal anterior de rodilla y artrotomía pararrotuliana medial con prolongación subvasto int.
- Artroplastia unicompartimental de rodilla modelo PKR de Stryker:
- Componente femoral cementado nº 2.
- Componente tibial cementado nº 2 e inserto de 8 mm.
- Patela:
- Correcto balance mediolateral en flexión y extensión y adecuado tracking rotuliano.
- Se retira isquemia, hemostasia de vasos sangrantes y lavado abundante con SF.
- Cierre por planos.
- Drenaje aspirativo.
- Piel con grapas.
- Vendaje compresivo.
- EVOLUCIÓN: Durante el postoperatorio el paciente se ha mantenido afebril y hemodinámicamente estable. Ha presentado buen control del dolor con la analgesia pautada, sin evidenciarse deficits vasculonerviosos ni signos de TVP en el miembro intervenido. Ha tolerado correctamente la sedestación y la deambulación asistida. La herida quirúrgica no ha presentado signos de complicación local.
- Dada la evolución favorable la paciente es alta a domicilio.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Aplicar hielo sobre la rodilla operada 2-3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede  caminar con ayuda de un andador.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- NAPROXENO 550 mg / 8 horas vía oral.
- PARACETAMOL 1 gr/  8  horas, alterno  con anterior cada   4   horas si  dolor  intenso.
- OMEPRAZOL 20 mg/ 24  horas.
- ENOXAPARINA 40 mg  / 24 horas vía oral / 4 semanas

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar revisión en Admisión del  Hospital  para  CCEE Revisión Hospitalaria de COT (${DOCTOR}) en 4 semanas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

**Tratamiento al Alta — Ejercicios (opcional, toggle en UI):**

> Mismo bloque de ejercicios compartido por todas las prótesis de rodilla. Ver contenido completo en PTR Triathlon arriba.

##### `rpuc` — Revisión PUC (RPUC)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Rescate PUC ${LADO_F_UPPER} por prótesis dolorosa:
- Profilaxis antibiótica con 2 gr de CEFAZOLINA.
- Isquemia en raíz de muslo.
- Incisión longitudinal anterior de rodilla sobre cicatriz anterior y artrotomía pararrotuliana medial.
- Retirada de componentes de PUC anterior: componente tibial y femoral sin pérdida de stock óseo.
- Componente femoral CR nº 3 no cementado.
- Componente tibial nº 3 cementado MBT.
- Inserto tibial RP de nº 3 de 15 mm.
- Artroplastia de rótula cementada de 35 mm.
- Correcto balance mediolateral en flexión y extensión y adecuado tracking rotuliano que no precisa Ficat.
- Se retira isquemia, hemostasia de vasos sangrantes y lavado abundante con SF.
- Cóctel analgésico.
- Cierre por planos.
- Drenaje aspirativo.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentada.
- Aplicar hielo sobre la rodilla operada 2-3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede  caminar con ayuda de un andador.
- Puede requerir ayuda domiciliaria
- METAMIZOL  1 cápsula / 8 horas vía oral.
- PARACETAMOL 1 gr/  8  horas, alterno  con anterior cada   4   horas si  dolor  intenso.
- OMEPRAZOL 20 mg/ 24  horas.
- ENOXAPARINA 40 mg  / 24 horas vía oral / 4 semanas
- Revisión  en  CC EE de COT (${DOCTOR} ) en 4 semanas  para valoración y  seguimiento.
- Solicitar cita en  CCEE  del  Servicio  de  Rehabilitación  para inicio fisioterapia

CURAS LOCALES
- Curas planas cada 48-72 horas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias. Mover activamente los dedos de la extremidad operada.
```

**Tratamiento al Alta — Ejercicios (opcional, toggle en UI):**

> Mismo bloque de ejercicios compartido por todas las prótesis de rodilla. Ver contenido completo en PTR Triathlon arriba.

<a id="categoría-lca"></a>

#### LCA (12 plantillas)

##### `lca_procinch` — LCA ProCinch anatómico ST-RI

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Se realiza exploración bajo anestesia previa que confirma la lesión de LCA.
- Obtención y preparación de plastia autóloga ST-RI.
- Fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin lesiones meniscales ni condrales.
- Compartimento externo: sin lesiones meniscales ni condrales.
- Ligamentoplastia LCA 4ST-RI con anclaje femoral Procinch y tibial con TIF Biosteon 9*35 mm.
- Drenaje aspirativo intraarticular.
- Cierre por planos de la fascia del sartorio y TCS.
- Piel con grapas y vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS

Recomendaciones:
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas apoyo parcial de la pierna intervenida y  movilidad   libre   según tolerancia.
- Realizar ejercicios de cuádriceps y movilidad de la rodilla.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- INHIXA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_procinch_allinside` — LCA ProCinch anatómico ALL-INSIDE

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Rotura crónica LCA RD.
- Anestesia raquídea.
- Profilaxis con 2 gr cefazolina.
- Isquemia muslo ${LADO_M} 250 mmHg.
- Abordaje longitudinal sobre pata de ganso. Disección por planos. Fasciotomía sartorio y obtención de plastia ST.
- Preparación de plastia cuádruple de ST con 2 ProCinch (Stryker) de 7 cm longitud x 9 mm diámetro.
- Tiempo artroscópico: portales artroscópicos habituales: AL, AM y AM accesorio.
- No lesiones meniscales ni condrales.
- Realización de TF fuera-dentro con broca retrógrada Versitomic RR de 9 mm x 25 mm.
- Realización de TT fuera-dentro con broca retrógrada Versitomic RR de 9 mm x 30 mm.
- Ampliación portal AM accesorio e introducción de la plastia por el mismo hacia TF primero y TT posteriormente.
- Se introduce 20 mm de plastia en cada túnel y se tensiona bidireccionalmente a 20º flexión y cajón posterior.
- Lavado articular abundante.
- Se deja drenaje intraarticular.
- Retirada de isquemia y cierre por planos.
- Se infiltra zona donante y portales con cóctel analgésico con 5 mg cloruro mórfico y 10 cc ropivacaína.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS

Recomendaciones:
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas apoyo parcial de la pierna intervenida y  movilidad   libre   según tolerancia.
- Realizar ejercicios de cuádriceps y movilidad de la rodilla.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- INHIXA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_procinch_lemaire` — LCA ProCinch + Lemaire

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Obtención de plastia autóloga ST-RI.
- Fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: rotura en asa de cubo del cuerpo y CPMI que se sutura con 3 puntos de fast-fix y 1 punto fuera dentro con ticron 2.
- Compartimento externo: sin lesiones meniscales ni condrales.
- Ligamentoplastia 4 ST-RI con anclaje femoral Procinch y tibial con tornillo interferencial de 9*28 mm.
- Drenaje aspirativo intraarticular.
- Cierre por planos de la fascia del sartorio y TCS.
- Se infiltra portales y en región intraarticular con ropivacaína y 5 mg de cloruro mórfico.
- Piel con grapas y vendaje compresivo.
- Plastia de refuerzo extraarticular con técnica de Lemaire modificada manteniendo inserción distal de plastia de banda iliotibial y fijada en fémur con TIF Biosteon 7*28 mm.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS

Semana 0º-2ª:
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Ejercicios isométricos, de cuádriceps  y  EPE desde el  inicio.
- Movilidad rodilla libre según tolerancia.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Descarga  sin  apoyo  haciendo  hincapié  en la obtención  de  la extensión  completa de la rodilla en la fase postoperatoria  temprana.
- A la semana  cura de la herida y   las 2 semanas retirada de  puntos de sutura.

Semana 3ª:
- Apoyo  del  50% del  peso  corporal  con aumento progresivo.
- Ejercicios de  flexo-extensión con  incremento  gradual.
- Bicicleta estática

Semana 4ª:
- Carga total.
- BA  mínimo 0º-90º.
- Conducción.

Semana 8ª:
- Se debe haber conseguido  BA  completo.
- Seguir fortalecimiento muscular  en  gimnasio.
- 4º mes: Inicio  de carrera  continua suave.
- 6º mes: Retorno  a la actividad deportiva, incluido deportes de  contacto.
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_procinch_sutura` — LCA ProCinch + sutura meniscal

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Se realiza exploración bajo anestesia previa que confirma la lesión de LCA.
- Obtención y preparación de plastia autóloga ST-RI.
- Fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin lesiones meniscales ni condrales.
- Compartimento externo: sin lesiones meniscales ni condrales.
- Ligamentoplastia LCA 4ST-RI con anclaje femoral Procinch y tibial con TIF Biosteon 9*35 mm.
- Drenaje aspirativo intraarticular.
- Cierre por planos de la fascia del sartorio y TCS.
- Piel con grapas y vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas SIN  APOYO  inicial de la pierna intervenida:
- Semana 0 – semana 3: descarga completa.
- Semana 3 – semana 6: carga parcial ayudado  de bastones.
- A partir  semana 6: puede caminar libremente sin  bastones (apoyo  completo).
- Aumento  progresivo  de la  movilidad para protección de la sutura meniscal:
- Semana 0 - semana 2: 0º a 60º.
- Semana 2 - semana 4: 0º  a 90º.
- Semana 4- semana 6: 90º a 120º.
- A partir  semana 6: movilidad libre.
- Realizar ejercicios isométricos de cuádriceps y elevación con  pierna extendida.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_procinch_reinsercion` — LCA ProCinch + reinserción raíz meniscal posterior

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Se realiza CAR previa bajo que confirma la lesión de LCA.
- Obtención y preparación de plastia autóloga ST-RI.
- Fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin lesiones meniscales ni condrales.
- Compartimento externo: avulsión de la raíz meniscal de CPML tipo 4 (lesión oblicua completa con desinserción de la raíz). Se realiza reinserción anatómica con punto de sutura técnica transtibial y fijación distal en cortical anterior con botón.
- Ligamentoplastia LCA 4ST-RI con anclaje femoral Procinch y tibial con TIF Biosteon 9*28 mm.
- Drenaje aspirativo intraarticular.
- Cierre por planos de la fascia del sartorio y TCS.
- Piel con grapas y vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Se va a proceder de protección  de la reparación  quirúrgica y  posteriormente a un  protocolo  de carga  progresiva de la rodilla intervenida.
- Puede caminar con ayuda de 2 muletas SIN  APOYO  inicial de la pierna intervenida:
- Semana 0 – semana 6: descarga completa.
- Semana 6 – semana 8: carga parcial ayudada  de bastones.
- A partir  semana 8: puede caminar libremente sin  bastones (apoyo  completo).
- Aumento  progresivo  de la  movilidad para protección de la sutura meniscal:
- Semana 0 - semana 2: 0º a 90º.
- A partir de la semana 2 se procede a un  incremento  progresivo  de la movilidad según   tolerancia.
- Realizar ejercicios isométricos de cuádriceps y elevación con  pierna extendida.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Evitar  los ejercicios de flexión  profunda de la rodilla,  como  la prensa o  sentadillas,  por  un  periodo  no  menor a  4  meses.
- Retorno a la actividad deportiva a partir de los 6  meses de la cirugía.
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para inicio  de la fisioterapia lo  antes posible a fin  de trabajar la movilidad pasiva de la rodilla intervenida y  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_hth` — LCA Hueso-Tendón-Hueso (HTH)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- CAR diagnóstica que confirma rotura completa de LCA.
- Incisión longitudinal desde polo inferior de rótula a borde medial de TTA. Apertura del paratenon y obtención plastia HTH de 10 mm de anchura del tendón rotuliano y 2 pastillas óseas en los extremos 8*25 mm en rótula y 9*30 mm en TTA.
- Ligamentoplastia LCA con autoinjerto HTH homolateral con técnica anatómica:
- Túnel femoral ciego de 8*30 mm con fresas flexibles de Clancy desde portal AM accesorio.
- Túnel tibial de 9 mm * 35 mm realizado a 55º.
- Ascenso de la plastia HTH en sentido retrógrado y fijación túnel femoral con tornillo interferencial Biorci HA 7*25 mm y de 8*30 mm en túnel tibial.
- Se comprueba estabilidad del injerto y ausencia de roce en escotadura intercondílea con extensión completa.
- Lavado articular.
- Cierre por planos.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas SIN  APOYO  inicial de la pierna intervenida:
- Semana 0 – semana 3: descarga completa.
- Semana 3 – semana 6: carga parcial ayudado  de bastones.
- A partir  semana 6: puede caminar libremente sin  bastones (apoyo  completo).
- Aumento  progresivo  de la  movilidad para protección de la sutura meniscal:
- Semana 0 - semana 2: 0º a 60º.
- Semana 2 - semana 4: 0º  a 90º.
- Semana 4- semana 6: 90º a 120º.
- A partir  semana 6: movilidad libre.
- Realizar ejercicios isométricos de cuádriceps y elevación con  pierna extendida.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_aum_am` — LCA Aumentación AM

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Se realiza CAR diagnóstica bajo anestesia previa apreciándose rotura del fascículo AM del LCA, con integridad del fascículo PL.
- Obtención de plastia autóloga cuádruple de tendones de pata de ganso ST a través de incisión oblicua en cara anterointerna de tercio proximal de tibia.
- Fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin lesiones meniscales ni condrales.
- Compartimento externo: sin lesiones meniscales ni condrales.
- Limpieza de la escotadura condílea con sinoviotomo y vaporizador conservando fascículo PL del LCA nativo.
- Realización de túnel tibial de 8 mm.
- Realización de túnel femoral a través del túnel tibial con guía over de top de 8 mm * 35 mm (resto hasta 50 mm con broca de 4,5 mm).
- Plastia ST doble con anclaje femoral endobutton 25 mm y tibial con tornillo interferencial de 9*20 mm.
- Drenaje aspirativo intraarticular.
- Cierre por planos de la fascia del sartorio y TCS.
- Se infiltra portales y en región intraarticular con ropivacaína y 5 mg de cloruro mórfico.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas apoyo parcial de la pierna intervenida y  movilidad   libre   según tolerancia.
- Realizar ejercicios de cuádriceps y movilidad de la rodilla.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- METAMIZOL  575 mg/ 8  horas  (alterno  con  anterior  cada  4   horas),  si dolor intenso.
- PARACETAMOL 1 gr cada 8 horas
- BEMIPARINA 3500 UI/24 horas vía subcutánea.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (TRAP) a  las  2 semanas,  6  semanas  y  4  meses  desde la cirugía   para seguimiento.
- Solicitar  cita en Servicio  de  Rehabilitación de su  área de referencia para inicio de fisioterapia.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_aum_pl` — LCA Aumentación PL

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Se realiza CAR diagnóstica bajo anestesia previa apreciándose rotura del fascículo PL del LCA, con integridad del fascículo AM.
- Obtención de plastia autóloga de HTH a través de incisión central de polo inf rótula a TTA.
- Fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: rotura longitudinal periférica del CPMI que se sutura con 3 puntos de fast-fix.
- Compartimento externo: sin lesiones meniscales ni condrales.
- Limpieza de la escotadura condílea con sinoviotomo y vaporizador conservando fascículo AM del LCA nativo.
- Realización de túnel femoral ciego de 9*30 mm a través del portal AM accesorio.
- Realización de túnel tibial de 9 mm realizado a 55º en región post de la huella tibial del LCA. Respetando fibras del fascículo AM.
- Ascenso de la plastia HTH en sentido retrógrado y fijación túnel femoral con tornillo interferencial Biorci HA 7*25 mm y de 8*30 mm en túnel tibial.
- Se comprueba estabilidad del injerto y ausencia de roce en escotadura intercondílea con extensión completa.
- Se infiltra portales y en región intraarticular con ropivacaína y 5 mg de cloruro mórfico.
- Drenaje aspirativo intraarticular.
- Lavado articular, cierre por planos, piel con grapas y vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas apoyo parcial de la pierna intervenida y  movilidad   libre   según tolerancia.
- Realizar ejercicios de cuádriceps y movilidad de la rodilla.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- METAMIZOL  575 mg/ 8  horas  (alterno  con  anterior  cada  4   horas),  si dolor intenso.
- PARACETAMOL 1 gr cada 8 horas
- BEMIPARINA 3500 UI/24 horas vía subcutánea.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (TRAP) a  las  2 semanas,  6  semanas  y  4  meses  desde la cirugía   para seguimiento.
- Solicitar  cita en Servicio  de  Rehabilitación de su  área de referencia para inicio de fisioterapia.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_rescate` — LCA Rescate — revisión

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Se prepara plastia de banco de tejidos HTH con pastilla ósea para fémur de 9*25 mm y para tibia de 11*30 mm.
- Fondos de saco cuadricipitales: sin alteraciones de interés.
- Compartimento interno: secuelas de meniscectomía parcial del CPMI de cirugía previa.
- Compartimento externo: secuelas de meniscectomía parcial del CAME de cirugía previa. Condropatía grado 2 de zona de carga del cóndilo femoral ext.
- Limpieza de la escotadura condílea con sinoviotomo y vaporizador.
- Condiloplastia con fresa motorizada por cierre de la misma.
- Realización de túnel femoral a través de portal medial accesorio de 9 mm * 40 mm.
- Realización de túnel tibial de 11*35 mm.
- Fijación de la plastia: femoral con TIF Biorci-HA 7*25 mm y tibial con TIF Biorci-HA 10*30 mm.
- Se comprueba ausencia de roce de la plastia en borde de la escotadura femoral tras condiloplastia realizada.
- Drenaje aspirativo intraarticular.
- Cierre por planos de la fascia del sartorio y TCS.
- Se infiltra portales y en región intraarticular con ropivacaína y 5 mg de cloruro mórfico.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas apoyo parcial de la pierna intervenida y  movilidad   libre   según tolerancia.
- Realizar ejercicios de cuádriceps y movilidad de la rodilla.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg / 8 horas vía oral.
- METAMIZOL  575 mg/ 8  horas  (alterno  con  anterior  cada  4   horas),  si dolor intenso.
- BEMIPARINA 3500 UI/24 horas vía subcutánea.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (${DOCTOR}) en  2/3 semanas  para ver evolución y retirar puntos.
- Al  alta solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_rescate_hth_lemaire` — LCA Rescate — HTH banco + Lemaire

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Rescate de ligamentoplastia de LCA de la rodilla ${LADO_F}.
- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Exploración bajo anestesia que confirma rotura completa de la plastia autóloga previa de LCA.
- Rotura longitudinal en asa de cubo del CPMI luxada que se reduce y se sutura con 3 puntos de fast-fix.
- Preparación de la plastia de HTH de banco de tejidos con pastillas en fémur 7*25 y tibia 9*30 mm y rescate ligamentoplastia con técnica anatómica:
- Túnel femoral 30*9 mm.
- Túnel tibial progresivo hasta 10 mm a 55º.
- Ascenso de la plastia HTH en sentido retrógrado y fijación túnel femoral con tornillo interferencial Biosteon 7*23 mm y de 9*28 mm en túnel tibial.
- Se comprueba estabilidad del injerto y ausencia de roce en escotadura intercondílea con extensión completa.
- Plastia de refuerzo extraarticular de rodilla (Lemaire modificado) manteniendo inserción distal de banda iliotibial y fijada en fémur con TIF Biosteon 7*28 mm.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS

Semana 0º-2ª:
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Ejercicios isométricos, de cuádriceps  y  EPE desde el  inicio.
- Movilidad rodilla libre según tolerancia.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Descarga  sin  apoyo  haciendo  hincapié  en la obtención  de  la extensión  completa de la rodilla en la fase postoperatoria  temprana.
- A la semana  cura de la herida y   las 2 semanas retirada de  puntos de sutura.

Semana 3ª:
- Apoyo  del  50% del  peso  corporal  con aumento progresivo.
- Ejercicios de  flexo-extensión con  incremento  gradual.
- Bicicleta estática

Semana 4ª:
- Carga total.
- BA  mínimo 0º-90º.
- Conducción.

Semana 8ª:
- Se debe haber conseguido  BA  completo.
- Seguir fortalecimiento muscular  en  gimnasio.
- 4º mes: Inicio  de carrera  continua suave.
- 6º mes: Retorno  a la actividad deportiva, incluido deportes de  contacto.
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_reparacion`
**LCA Reparación (InternalBrace)**

**Hoja operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M}.
- Abordajes AL y AM.
- Fondos de saco cuadricipitales: sin alteraciones.
- Compartimento interno: sin lesiones meniscales ni condrales.
- Compartimento externo: sin lesiones meniscales ni condrales.
- Compartimento central: se aprecia lesión LCA (Sherman tipo I-II) con buena calidad de remanente ligamentoso. Fijación femoral mediante Swivelock cargado con Fibertape (Internalbrace). Fijación tibial mediante Swivelock tras túnel transtibial con broca de 3.5 (Flipcutter).
- Cierre por planos.
- Piel con grapas y vendaje compresivo.
```

**Tratamiento al alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas SIN  APOYO  inicial de la pierna intervenida:
- Semana 0 – semana 3: descarga completa.
- Semana 3 – semana 6: carga parcial ayudado  de bastones.
- A partir  semana 6: puede caminar libremente sin  bastones (apoyo  completo).
- Aumento  progresivo  de la  movilidad para protección de la reparación ligamentosa:
- Semana 0 - semana 2: 0º a 60º.
- Semana 2 - semana 4: 0º  a 90º.
- Semana 4- semana 6: 90º a 120º.
- A partir  semana 6: movilidad libre.
- Realizar ejercicios isométricos de cuádriceps y elevación con  pierna extendida.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 3 semanas.

REVISIÓN
- Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `lca_allinside_arthrex` — LCA All-Inside ST Arthrex (no registrada en UI)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia raquídea.
- Profilaxis antibiótica con 2 gr de cefazolina.
- Isquemia en raíz de muslo ${LADO_M} 250 mmHg.
- Abordaje longitudinal sobre pata de ganso. Disección por planos. Fasciotomía sartorio y obtención de plastia ST.
- Preparación de plastia cuádruple de ST con 2 Tightrope (Arthrex) de 7 cm longitud * 9 mm diámetro.
- Tiempo artroscópico: portales artroscópicos habituales: AL, AM y AM accesorio.
- No lesiones meniscales ni condrales.
- Realización de túnel femoral fuera dentro con broca retrógrada Flipcutter (Arthrex) de 9 mm * 25 mm.
- Realización de túnel tibial fuera dentro con broca retrógrada Flipcutter (Arthrex) de 9 mm * 30 mm.
- Ampliación portal AM accesorio e introducción de la plastia por el mismo hacia TF primero y TT posteriormente.
- Se introduce 20 mm de plastia en cada túnel y se tensiona bidireccionalmente a 20º flexión y cajón posterior.
- Fijación femoral y tibial con Tightrope (Arthrex).
- Lavado articular abundante.
- Se deja drenaje intraarticular.
- Retirada de isquemia y cierre por planos.
- Se infiltra zona donante y portales con cóctel analgésico con 5 mg cloruro mórfico y 10 cc ropivacaína.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Aplicar  hielo  sobre  vendaje  4 veces al  día  durante 30 minutos.
- Puede caminar con ayuda de 2 muletas SIN  APOYO  inicial de la pierna intervenida:
- Semana 0 – semana 3: descarga completa.
- Semana 3 – semana 6: carga parcial ayudado  de bastones.
- A partir  semana 6: puede caminar libremente sin  bastones (apoyo  completo).
- Aumento  progresivo  de la  movilidad para protección de la reparación ligamentosa:
- Semana 0 - semana 2: 0º a 60º.
- Semana 2 - semana 4: 0º  a 90º.
- Semana 4- semana 6: 90º a 120º.
- A partir  semana 6: movilidad libre.
- Realizar ejercicios isométricos de cuádriceps y elevación con  pierna extendida.
- Movilizaciones pasivas de  rótula 4/5 veces al  día  durante  15 minutos.
- Puede requerir ayuda domiciliaria
- ENANPLUS  75 mg/25 mg  / 8 horas vía oral.
- PARACETAMOL 1 gr cada 8 horas
- ENOXAPARINA 40 mg /24 horas vía subcutánea  durante 3 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN

Antes de irse de alta  del  hospital:
- Solicitar  cita en  Admisión  de  Consultas Externas para revisión en CC EE  de  COT (${DOCTOR})  en  2/3   semanas  para ver evolución.
- Solicitar  cita en  Servicio de  Rehabilitación  para  seguimiento  postoperatorio.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

<a id="categoría-rodilla_osteo"></a>

#### Osteotomías y Cartílago (8 plantillas)

##### `rodilla_ovt` — Osteotomía valguizante de tibia (apertura medial)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Abordaje medial oblicuo anterior a los isquiotibiales. Localización de pata de ganso y LLI
- Sección de tercio anterior y distal de LLI
- Osteotomía transversa medial de apertura de tibia tras control por Rx (3-3,5 cm distal a línea articular) y corte con sierra parando 1 cm antes de la cortical lateral
- Osteotomía vertical (110º con respecto a la osteotomía horizontal) tras la TTA separando el tendón rotuliano hasta proximal
- Con pinza reguladora vamos ampliando los grados lentamente (15-20 min mientras realizamos la extracción de cresta) hasta conseguir 12º (hipercorrección de los 11,5º previstos)
- Extracción de cresta ilíaca ${LADO_F} a escoplo: 2 cuñas de 1,3 cm + esponjosa. Lavado, drenaje y cierre
- Introducción de las dos cuñas de base de 1,3 cm y esponjosa
- Colocación de placa TOMOFIX de Synthes tamaño Small, según técnica quirúrgica (tornillos bloqueados proximales bicorticales, tornillo de compresión para aproximación de la placa y sustitución por tornillo bloqueado, tornillos bloqueados distales bicorticales)
- Control por escopia comprobando el eje mecánico pasando por el punto Fujisawa con barra
- Lavado, drenaje y cierre por planos
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado
- Aplicar hielo sobre la rodilla operada 2-3 veces al día durante 20 minutos
- Mover activamente los dedos de la extremidad operada
- Realizar los ejercicios que su médico le ha explicado, permitiendo la flexoextensión libre de la rodilla
- NO APOYO DE LA PIERNA INTERVENIDA DURANTE 3 SEMANAS, después comenzará carga parcial otras 3 semanas y tras ello inicio de carga completa
- Paracetamol 1 g / 8 horas vía oral
- Metamizol 575 mg 1 caps / 8 horas, alterno con anterior cada 4 horas si dolor intenso
- Omeprazol 20 mg / 24 horas
- Bemiparina 3500 UI / 24 horas vía subcutánea / 6 semanas


CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias
```

##### `rodilla_ovt_slope` — OVT + corrección pendiente posterior

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Decúbito supino.
- Isquemia en raíz del muslo.

- 1º TIEMPO CAR:
- Portales tradicionales anteromedial y anterolateral
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía II en surco troclear
- Compartimento interno: rotura en flap desde el cuerno posterior al cuerpo del menisco interno y rotura de la región más anterior del mismo menisco que se reseca y regulariza con pinzas y motor
- Pivote central: rotura del LCA con signo del cíclope en fémur. Se reseca
- Compartimento externo: condropatía II, rotura del borde del cuerpo del ME

- 2º TIEMPO OSTEOTOMÍA:
- Control por escopia.
- Abordaje medial oblicuo. Localización del LLI
- Despegamos con periostótomo parte del LLI para dejar libre la zona de osteotomía. Localizamos borde posterior del LLI y desperiostizamos la cortical posteromedial de la tibia
- Retirada de los hilos de la plastia por el túnel tibial
- Osteotomía transversa medial de apertura de tibia tras control por Rx (3-3,5 cm distal a línea articular) y corte con sierra parando 1 cm antes de la cortical lateral
- Osteotomía vertical (110º con respecto a la osteotomía horizontal) tras la TTA separando el tendón rotuliano hasta proximal
- Introducción de los escoplos gradualmente introduciendo cada uno 1 cm menos que el anterior. La introducción de los mismos toma dirección de posterior a lateral y más anterior para poder disminuir la pendiente sin alterar la altura de la patela
- Colocación de placa ACTIVMOTION DE MEDCOMTECH tamaño Small (tornillos bloqueados proximales bicorticales, tornillo de compresión de cortical en diáfisis y los otros dos bloqueados)
- Control por escopia comprobando disminución de la pendiente y corrección del varo
- Lavado, drenaje y cierre por planos
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado
- Aplicar hielo sobre la rodilla operada 2-3 veces al día durante 20 minutos
- Mover activamente los dedos de la extremidad operada
- Realizar los ejercicios que su médico le ha explicado, permitiendo la flexoextensión libre de la rodilla
- NO APOYO DE LA PIERNA INTERVENIDA DURANTE 3 SEMANAS, después comenzará carga parcial otras 3 semanas y tras ello inicio de carga completa
- Paracetamol 1 g / 8 horas vía oral
- Metamizol 575 mg 1 caps / 8 horas, alterno con anterior cada 4 horas si dolor intenso
- Omeprazol 20 mg / 24 horas
- Bemiparina 3500 UI / 24 horas vía subcutánea / 6 semanas


CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias
```

##### `rodilla_fulkerson` — Osteotomía TTA tipo Fulkerson

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Manguito de isquemia en raíz del muslo.
- Profilaxis antibiótica con 2 g cefazolina iv.

- 1º TIEMPO (CAR):
- Condropatía faceta medial patela grado III, subluxación lateral, tróclea displásica, con tracking alterado
- Compartimento medial: condropatía tibial grado II-III
- Pivote central: LCA competente
- Compartimento lateral: meniscectomía cuerpo y cuerno anterior de ME, condropatía tibial grado II-III

- 2º TIEMPO:
- Incisión longitudinal rodilla anterior desde polo inferior de la rótula hasta 6-7 cm distales a TTA
- Desperiostizamos al borde lateral de la cresta tibial y marcamos la entrada de osteotomía por medial. Desperiostizamos 6-7 cm distal a TTA
- Con AK marcamos la entrada por anteromedial (1 cm de grosor desde TTA) y salida por posterolateral con cuidado de no dar con estructuras vasculonerviosas. Acabamos en apex distal de 2-3 mm
- Con sierra iniciamos cortical medial y continuamos con escoplo
- Visualizamos tendón rotuliano y marcamos por proximal el nivel de osteotomía y con escoplo lo hacemos
- Medializamos 1 cm, descenso de 2-3 mm y fijamos con dos tornillos de 4,5 cm hasta cortical posterior, divergentes
- Realizamos de nuevo CAR para visualizar el tracking y realizamos FICAT del alerón externo con tijera
- Se comprueba flexión a 90º con buen tracking y fijación
- Drenaje, cierre por planos. Vendaje
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado
- Aplicar hielo sobre la rodilla operada 2-3 veces al día durante 20 minutos
- Mover activamente los dedos de la extremidad operada
- Realizar los ejercicios que su médico le ha explicado: isométricos de cuádriceps, movilización de rótula horizontal y vertical y elevación con pierna extendida
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Puede caminar con ayuda de bastones con apoyo PARCIAL de la pierna intervenida
- Mantener ortesis de inmovilización con balance articular limitado de 0º a 45º durante 3 semanas y después movilidad libre
- Metamizol 1 cápsula / 8 horas vía oral
- Ibuprofeno 600 mg / 8 horas, alterno con anterior cada 4 horas si dolor intenso
- PARACETAMOL 1 gr cada 8 horas
- Omeprazol 20 mg / 24 horas
- Bemiparina 3500 UI 1 jeringa / 24 horas vía subcutánea / 6 semanas
- Solicitar cita con RHB al alta

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (${DOCTOR}) en 3 semanas para ampliar arco movilidad y seguimiento

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias
```

##### `rodilla_mosaico_ovt` — Mosaicoplastia + OVT

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Decúbito supino con pernera en pierna ${LADO_F}.
- Isquemia en raíz del muslo.
- Control por escopia.

- 1º TIEMPO CAR:
- Portales habituales AM y AL.
- Compartimento FP: condropatía II en patela.
- Compartimento FTM: lesión OC en zona de carga de 25 mm × 20 mm aprox. Rotura en flap de cuerpo de ML que se regulariza con pinzas y motor.
- Pivote central: LCA íntegro y competente.
- Compartimento FTL: sin hallazgos.

- 2º TIEMPO OSTEOTOMÍA VALGUIZANTE DE TIBIA DE APERTURA MEDIAL:
- Incisión medial.
- Osteotomía de apertura de 8º sin invadir cortical lateral.
- Placa ActivMotion de NewClip talla 2.
- Control por escopia.

- 3º TIEMPO MOSAICOPLASTIA:
- Toma de 3 autoinjertos osteocondrales de 10, 8 y 8 mm (dos se toman de zona medial del CFM y uno de CFL) según técnica habitual con sistema Arthrex.
- Implantación de dichos injertos en zona defectuosa con puentes de 1-2 mm entre ellos quedando a ras de su cartílago sano. Profundidad de los injertos de 15 mm.
- Lavado con SF. Cierre.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2-3 veces al día durante 20 minutos
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Puede caminar con ayuda de 2 muletas SIN APOYO de la pierna intervenida hasta nueva orden
  * Semana 0-6: NO PUEDE APOYAR. Descarga completa
  * Semana 6-12: inicio parcial y progresivo de la carga
- Realizar ejercicios isométricos de cuádriceps
- Movilidad libre de rodilla sin apoyo
- Enanplus 1 comp / 8 horas vía oral alternando con Metamizol si persistencia del dolor
- PARACETAMOL 1 gr cada 8 horas
- Enoxaparina Rovi 40 mg / 24 horas vía subcutánea durante 4 semanas
- Retirada de puntos por ATS DE ZONA en 12-15 días

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Revisión en CCEE de COT (${DOCTOR}) en 3 semanas para ver evolución

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `rodilla_lfpm_tta` — Reconstrucción LFPM + osteotomía TTA (luxación rótula)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- LRR RÓTULA ${LADO_F}
- Profilaxis antibiótica con 2 g de cefazolina
- Isquemia en raíz de muslo

- 1º TIEMPO (CAR):
- Portal AL y accesorio suprapatelar medial.
- Compartimento externo y medial sin alteraciones.
- Pivote central con LCA competente e íntegro.
- Rótula con condropatía II-III faceta lateral y II-III surco. Fragmentos mediales que intentamos retirar por artroscopia siendo imposible y necesitando artrotomía medial para su exéresis.

- 2º TIEMPO:
- Incisión medial a la TTA para extracción de recto interno con tenótomo.
- Osteotomía de 6 cm descendiendo 0,5 cm y ligera medialización. Fijación con dos tornillos canulados proximales, placa de tercio de caña en región de osteotomía distal transversa con dos tornillos.

- 3º TIEMPO:
- Abordaje medial y superior a la rótula disecando espacio bajo la capa 1.
- Abordaje sobre epicóndilo y tubérculo del aductor. Se diseca espacio bajo la capa 1 haciéndolo comunicar con el anterior.
- Reconstrucción del LFPM usando sistema de fijación de Arthrex en rótula y fijación con tornillo interferencial del mismo sistema de 6×23 mm en CFI (en zona entre tubérculo del aductor y epicóndilo comprobado por escopia y con referencia el punto de Schöttle) previa comprobación de la tensión e isometría del mismo. Fijación a 30º.
- Comprobación de lateralización <1 cm.
- Cierre por planos de las heridas. Piel con grapas. Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado
- Crioterapia: aplicar hielo sobre la rodilla operada 3 veces al día durante 20-25 minutos
- Mover activamente los dedos de la extremidad operada
- Realizar los ejercicios isométricos que su médico le ha explicado
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Retirada de puntos de sutura una vez cicatrizada la herida quirúrgica (12-14 días aproximadamente)

MEDICACIÓN
- PARACETAMOL 1 gr cada 8 horas

MOVILIDAD:
  * 0-2 semana: ejercicios pasivos de movilidad de rodilla con ortesis bloqueada a 0-30º
  * 2-3ª semana: aumento del balance articular a 0-60º
  * 3-6ª semana: aumento del balance articular a 0-90º
  * A partir de la 6ª semana: retirada de ortesis y movilidad libre

CARGA:
  * 0-3 semanas: descarga completa
  * 3-8 semanas: inicio de carga muy parcial y progresiva
  * A partir de semana 8: carga completa

INICIO ACTIVIDAD DEPORTIVA:
  * Bicicleta: 2º mes
  * Natación: 3º mes
  * Retorno actividad deportiva: 6º mes

CURAS LOCALES
- Curas planas cada 48-72 horas.
```

##### `rodilla_car_dlo_newclip` — CAR + DLO (doble nivel) — Actimotion S (New Clip/PSI)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

CAR ${LADO_F_UPPER} + osteotomía a doble nivel (fémur y tibia) por genu varo severo MII realizada con plantillas personalizadas de corte PSI de New Clip
- CAR ${LADO_F_UPPER} sin isquemia:
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía de la tróclea femoral y patela grado 2.
- Compartimento interno: condropatía grado 4 de toda zona carga de cóndilo femoral int y meseta tibial int. Ausencia casi completa menisco medial.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Osteotomía biplanar lateral de fémur distal ${LADO_M} de sustracción (6º) fijada con placa Actimotion S con 4 tornillos bloqueados distales, 3 proximales y 1 tornillo que cruza osteotomía.
- Isquemia en raíz muslo ${LADO_M}:
- OVT biplanar de adición interna (8º) fijada con placa Actimotion S con 4 tornillos bloqueados distales y 4 proximales. Relleno de la cuña de apertura con injerto autólogo tricortical de cresta iliaca y chips de esponjosa.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos, tobillo y rodilla de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas SIN APOYO de la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y movilidad libre de la rodilla.
- Puede requerir ayuda domiciliaria.
- Naproxeno 550 mg / 8 horas vía oral.
- Paracetamol 1 g cada 8 horas vía oral alterno con Naproxeno cada 4 horas.
- Omeprazol 20 mg / 24 horas.
- Bemiparina 3500 UI / 24 horas vía subcutánea.
- Curas por DUE de zona cada 48/72 horas.
- Revisión en CCEE de COT (${DOCTOR}) en 3 semanas para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `rodilla_car_ovt_newclip` — CAR + OVT adición — Actimotion S (New Clip)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

CAR ${LADO_F_UPPER} + osteotomía de adición valguizante de tibia ${LADO_F_UPPER}
- Isquemia en muslo ${LADO_M}.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía de la tróclea femoral grado 4.
- Compartimento interno: rotura degenerativa del cuerpo y cuerno posterior del menisco interno que se reseca y regulariza con pinzas y motor. Condropatía grado 4 de toda zona carga de cóndilo femoral int y meseta tibial int.
- Pivote central: LCA íntegro y competente.
- Compartimento externo: sin alteraciones.
- Extracción de injerto bicortical de cresta iliaca y chips de esponjosa.
- Incisión oblicua en tercio proximal y medial de tibia siguiendo dirección de los tendones isquiotibiales.
- Desinserción parcial de la inserción distal del fascículo superficial del LLI.
- Osteotomía biplanar de tibia respetando la TTA con sierra y completada con escoplo.
- Apertura de la cuña de forma progresiva hasta 16º y relleno de la misma con el injerto autólogo cortical y de esponjosa.
- Osteosíntesis con placa de osteotomía tibial medial proximal Actimotion S (New Clip) fijada con 4 tornillos proximales y 4 tornillos distales fijados a placa.
- Cierre por planos.
- Piel con grapas.
- Vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos, tobillo y rodilla de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas SIN APOYO de la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y movilidad libre de la rodilla.
- Puede requerir ayuda domiciliaria.
- Naproxeno 550 mg / 8 horas vía oral.
- Paracetamol 1 g cada 8 horas vía oral alterno con Naproxeno cada 4 horas.
- Omeprazol 20 mg / 24 horas.
- Bemiparina 3500 UI / 24 horas vía subcutánea.
- Curas por DUE de zona cada 48/72 horas.
- Revisión en CCEE de COT (${DOCTOR}) en 3 semanas para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

##### `rodilla_car_ovt_lca_medcontech` — CAR + OVT adición (Medcontech) + LCA

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

CAR + osteotomía de adición valguizante de tibia + ligamentoplastia LCA rodilla ${LADO_F}
- Isquemia en muslo ${LADO_M}.
- Portales tradicionales anteromedial y anterolateral.
- Articulación femoropatelar y fondos de saco cuadricipitales: condropatía grado 2 CFI, rotura degenerativa del asta post del menisco medial (meniscectomía parcial con pinzas y sinoviotomo), rotura completa LCA, y compartimento ext sin lesiones meniscales ni condrales.
- Incisión oblicua en tercio proximal y medial de tibia siguiendo dirección de los tendones isquiotibiales. Extracción de tendones recto int y semitendinoso.
- Desinserción parcial de la inserción distal del fascículo superficial del LLI.
- Osteotomía biplanar de tibia respetando la TTA con sierra y completada con escoplo.
- Apertura de la cuña de forma progresiva hasta 8º y relleno de la misma con hueso sintético.
- Osteosíntesis con placa de osteotomía tibial medial proximal de reconstrucción LCA de Medcontech fijada con 3 tornillos proximales y 3 tornillos distales fijados a placa.
- Ligamentoplastia LCA con 4ST-RI fijada en fémur con ProCinch y en tibia con TIF 10x35 mm.
- Cierre por planos, drenaje aspirativo, piel con grapas y vendaje compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Aplicar hielo sobre la articulación operada 2 - 3 veces al día durante 20 minutos.
- Mover activamente los dedos, tobillo y rodilla de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de 2 muletas SIN APOYO de la pierna intervenida.
- Realizar ejercicios isométricos de cuádriceps y movilidad libre de la rodilla.
- Puede requerir ayuda domiciliaria.
- Ibuprofeno 600 mg / 8 horas vía oral.
- Metamizol 575 mg cada 8 horas vía oral alterno con Ibuprofeno cada 4 horas.
- Omeprazol 20 mg / 24 horas.
- Bemiparina 3500 UI / 24 horas vía subcutánea.
- Curas por ATS de zona con Betadine cada 48/72 horas.
- Revisión en CCEE de COT (${DOCTOR}) en 3 semanas para ver evolución.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con el Hospital de Día en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario.
```

<a id="región-cadera"></a>

### Región: Cadera

<a id="categoría-ptc"></a>

#### Prótesis Cadera (3 plantillas)

##### `ptc_summit` — PTC Summit (DePuy)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Coxartrosis cadera ${LADO_F}.
- Profilaxis antibiótica con 2 gramos de cefazolina y 1 gramo IV de tranexámico.
- Decúbito lateral ${DECUBITO}.
- Incisión longitudinal sobre región trocantérica y vía abordaje Bauer.
- Capsulectomía, luxación de cabeza femoral y osteotomía del cuello.
- Artroplastia total cadera ${LADO_F} modelo Summit con cotilo Pinacle sector Gription no cementado nº 50, polietileno Marathon nº 50 +10º, vástago nº 6 no cementado estándar con cabeza de 28 mm +5 de cerámica.
- Se comprueba estabilidad de la artroplastia tras reducción en todos los planos.
- Cierre por planos con reinserción de musculatura glútea.
- Se administra 1 gramo de tranexámico en 50 cc de SF a nivel local.
- Piel con grapas.
- Apósito compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Aplicar hielo sobre la cadera operada 2-3 veces al día durante 20 minutos.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede  caminar con ayuda de un andador.
- Puede requerir ayuda domiciliaria

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575 mg / 8 horas vía oral.
- PARACETAMOL 1 gr/  8  horas, alterno  con anterior cada   4   horas si  dolor  intenso.
- OMEPRAZOL 20 mg/ 24  horas.
- ENOXAPARINA 40 mg  / 24 horas vía oral / 4 semanas

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar revisión en Admisión del  Hospital  para  CCEE Revisión Hospitalaria de COT (${DOCTOR}) en 4 semanas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ptc_zimmer` — PTC Zimmer (G7 + Taperloc)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Coxartrosis cadera ${LADO_F}.
- Profilaxis antibiótica con 2 gramos de cefazolina.
- Decúbito lateral ${DECUBITO}.
- Incisión longitudinal sobre región trocantérica y vía abordaje Hardinge.
- Capsulectomía, luxación de cabeza femoral y osteotomía del cuello.
- Artroplastia total cadera ${LADO_F} (Zimmer): cotilo G7 nº 48 press-fit, vástago Taperloc nº 7.5, inserto polietileno con ceja 10º y cabeza cerámica 32 +0 mm.
- Se comprueba estabilidad de la artroplastia tras reducción en todos los planos.
- Cierre por planos con reinserción de musculatura glútea.
- Drenaje aspirativo.
- Piel con grapas.
- Apósito compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de un andador o dos muletas
- ENANTYUM 1 cápsula /8 horas vía oral.
- PARACETAMOL 1gr/8 horas, alterno con anterior cada 4 horas si dolor intenso.
- OMEPRAZOL 20mg/24 horas.
- CLEXANE 40 mg/ cada 24 horas durante 30 dias.
- Puede requerir ayuda domiciliaria.

Curas y retirada de puntos de sutura/agrafes según informe de Enfermería.

REVISIÓN
- Antes de irse de alta, el paciente deberá solicitar revisión en Admisión del Hospital para CCEE Revisión Hospitalaria de COT (${DOCTOR}) en 4 semanas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ptc_stryker` — PTC Stryker (Trident + Accolade)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

Artroplastia total de cadera ${LADO_F} (Stryker: Trident + Accolade)
- Coxartrosis cadera ${LADO_F}.
- Decúbito lateral ${DECUBITO}. Anestesia raquimedular y sedación.
- Profilaxis ATB IV con cefazolina 2 g. Ác. tranexámico IV 1 g.
- Abordaje de Hardinge sobre cadera ${LADO_F}. Capsulectomía anterior.
- Artroplastia total de cadera con par polietileno-cerámica:
- Cotilo Trident de __ mm, estabilidad primaria con técnica line-to-line.
- Inserto de polietileno neutro.
- Vástago femoral Accolade nº 7, offset STD.
- Cabeza de cerámica de 32 mm, cuello +0.
- Lavado con abundante SSF. Infiltración con ác. tranexámico.
- Cierre por planos. Agrafes en piel.
- Apósito compresivo estéril.
- La intervención cursa sin incidencias. Simetría de MMII en decúbito supino.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado.
- Mover activamente los dedos de la extremidad operada.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede caminar con ayuda de un andador o dos muletas.
- Puede requerir ayuda domiciliaria.

MEDICACIÓN
- METAMIZOL 575 mg / 8 horas vía oral.
- PARACETAMOL 1 g / 8 horas, alterno con anterior cada 4 horas si dolor intenso.
- OMEPRAZOL 20 mg / 24 horas.
- ENOXAPARINA 40 mg / 24 horas vía subcutánea / 4 semanas.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar revisión en Admisión del Hospital para CCEE Revisión Hospitalaria de COT (${DOCTOR}) en 4 semanas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

<a id="categoría-cac"></a>

#### Artroscopia Cadera (1 plantillas)

##### `cac_labrum` — CAC: Reinserción labrum acetabular

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Decúbito supino.
- Profilaxis ATB.
- Mesa de tracción.
- Anestesia general.
- Control escopia.
- Portales ALP, ALD y anterior.

- Compartimento Central:
- Solo apertura longitudinal.
- Labrum ___________.
- Osteoplastia acetabular y reinserción de labrum con 4 anclajes.
- Osteoplastia cabeza femoral con control de escopia.
- Comprobación de maniobra de choque.
- Sutura capsular con ___________.
- Tiempo de tracción ___ min.
- Cierre de piel con prolene y grapa.
- Infiltración anestésica.
- Apósito compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la extremidad en alto durante las primeras 48 horas.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- IBUPROFENO 600 mg alternando con PARACETAMOL 1gr/ 8 horas vía oral según dolor.
- ENOXAPARINA 40 mg 1 jeringa / 24 horas vía subcutánea / 3 semanas.
- Retirada de puntos por su enfermero/a de referencia en el centro de salud en 7-10 días.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}  y  en  Servicio de  REHABILITACIÓN

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.

SIGA LAS SIGUIENTES RECOMENDACIONES DOMICILIARIAS:
- 1ª y 2ª SEMANAS
- Carga parcial con dos muletas.
- Frío local  durante 15min / varias veces al día. Nunca directamente sobre la piel.
- Todos los ejercicios deben realizarse en un rango de movilidad sin dolor.
- Realizar 10 repeticiones de cada grupo muscular de 3 a 4 veces al día.

Ejercicios:
- Evitar las elevaciones de la pierna recta (especialmente en pacientes con lesiones articulares).
- Flexión – Extensión de cadera: doblando la rodilla de la pierna afecta y deslizando el talón hacia la nalga tanto como sea posible. Cuando haya conseguido la máxima flexión, volver a poner la pierna recta.
- Rotación interna/externa: con la pierna recta realizar giros con los pies hacia dentro y hacia fuera. No forzar las rotaciones ( sobre todo tener precaución con la rotación interna ).
- Ejercicios circulatorios y de flexo – extensión del tobillo.
- Realizar cambios de posición frecuentes (sentarse/estirarse).
- Realizar contracciones isométricas de Cuádriceps e isquiotibiales, realizar contracciones simultáneas de ambos.
- Realizar contracciones isométricas de Abductores (cinta alrededor de los muslos y empujar hacia fuera).
- Realizar contracciones isométricas de Adductores (con una almohada entre los muslos).
- Realizar contracciones isométricas de Glúteos.
- En el momento que podamos sentarnos cómodamente, sin tensiones, podemos iniciar rodaje suave en bicicleta estática con el sillín alto para evitar flexión de la cadera >90 grados.
- No realizar movimientos bruscos.

Limitación del rango de movilidad:
- Extensión : 10 grados.
- Flexión : 90 grados.
- Abducción: 30 grados.
- Adducción: 30 grados.
- Rotación interna en flexión: 20 grados.
- Rotación externa en flexión : 70 grados.

RECUERDE: NO TODAS LAS ARTROSCOPIAS DE CADERAS SON IGUALES.
- Cada paciente evoluciona de forma diferente en función de la cirugía realizada, edad, el estado de salud previo y su
- capacidad para adaptarse a la Rehabilitación.
- Una complicación frecuente durante el programa de rehabilitación es la tendinitis del tendón del Psoas Iliaco. Cursa con dolor inguinal anterior y ocurre porque nos hemos excedido  en los ejercicios. En tal caso, debemos acudir al médico/fisioterapeuta para reconducir la rehabilitación.
- 3ª y 4ª SEMANAS
- Ir aumentando progresivamente la carga parcial con dos muletas de la pierna operada para conseguir soltar una muleta al final de la 3ª semana y sin muletas sobre la 4ª o 5ª semana.
- Frío local  durante 15min / varias veces al día. Nunca directamente sobre la piel.
- Todos los ejercicios deben realizarse en un rango de movilidad sin dolor.
- Realizar 10 repeticiones de cada grupo muscular de 3 a 4 veces al día.

Continuar con ejercicios previos y añadir los siguientes:
- Puente con dos piernas (pelvis neutra): tumbado boca arriba con las rodillas flexionadas y los pies apoyados en el suelo paralelos entre sí, elevar las caderas.
- Ejercicios de extensión de rodilla: colocar una toalla enrollada (15 cm de diámetro) bajo la rodilla de la pierna afectada. Poner la pierna recta sin perder el contacto del muslo con el rollo
- Abducción de caderas: con las piernas rectas, desplazar la pierna afectada lateralmente tanto como sea posible para después volver a juntarlas.
- (sigue en el siguiente apartado de recomendaciones generales)

RECOMENDACIONES GENERALES:
- Sentados en una silla, flexionar el cuerpo hacia delante progresivamente (teniendo en cuenta la tensión en la zona inguinal y no presencia de dolor).
- Bicicleta estática (10-15 min con mínima resistencia).
- Ejercicios en el agua, siempre que las heridas estén bien cicatrizadas y el entorno tenga fácil acceso (lo ideal es que el agua le llegue a la altura del pecho o cómo mínimo a la cintura):
- Caminar normalizando la marcha, talón – punta, lentamente para no hacer resistencia.
- Desplazarse lateralmente.
- Flexo-extensión de cadera, abducción de cadera y simular bicicleta suavemente.

Limitación del rango de movilidad:
- Extensión : 20 grados.
- Flexión : 120 grados.
- Abducción: 45 grados.
- Adducción: 45 grados.
- Rotación interna en flexión: 30 grados.
- Rotación externa en flexión : 90 grados.
```

<a id="categoría-ifc"></a>

#### Infiltración Cadera (1 plantillas)

##### `cadera_infiltracion` — Infiltración Cadera

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Sedoanalgesia.
- Paciente en decúbito supino.
- Bajo condiciones de estricta asepsia y control radiográfico se procede a infiltración de cadera ${LADO_F} mediante mepivacaína + corticoide.
- Apósito compresivo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Reposo relativo 24-48 horas.
- Analgesia habitual si precisa.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Retirar apósito pasadas las 6-8 horas de la intervención.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3-4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

<a id="región-ms"></a>

### Región: Miembro Superior

<a id="categoría-hombro_mr"></a>

#### Artroscopia Hombro (4 plantillas)

##### `hombro_cah` — CAH — Reparación artroscópica manguito rotador

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + locorregional. Profilaxis ATB. Decúbito lateral ${DECUBITO}.
- CAH ---.
- Portales habituales
- Glenohumeral: PLB, labrum y subescapular ok. Rotura supraespinoso grado  de Patte (porción anterolateral).
- Subacromial: bursectomía, se localiza rotura supraespinoso. Preparación footprint y reinserción supraespinoso con  Iconix Speed 2,3 (2 suturas). Acromioplastia anterior.
- Lavado articular, cierre de portales con agrafes e inmovilización con cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo durante 4-5 semanas. Puede retirarlo para aseo personal y para realizar ejercicios de flexo-extensión de codo así como pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Analgesia por elastómero prescrito por Servicio de Anestesia durante las primeras 24-48h. Continuar una vez retirado con Dexketoprofeno 25 mg v.o. 1/8 horas vía oral durante 4-5 días. Puede alternar con Metamizol caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 12-14 días
- Puede requerir reposo / ayuda domiciliaria
- Pedir cita con Servicio de RHB antes de marcharse de alta

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `hombro_cah_subescapular` — CAH — Con subescapular y doble hilera

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + locorregional. Profilaxis ATB. Decúbito lateral ${DECUBITO}.
- CAH ---.
- Portales habituales
- Glenohumeral: PLB y labrum ok, subescapular con rotura tipo II de Lafosse. Se realiza reparación tendón hueso con 1 Iconix 2,3 (2 cintas). Rotura supraespinoso grado II de Patte con mala calidad tisular e infiltración grasa.
- Subacromial: bursectomía, se localiza rotura supraespinoso. Preparación footprint (se fresa osteofito de tuberosidad mayor) y reinserción supraespinoso en doble hilera con 1 Iconix 2,3 medial (2 suturas) y 1 ReelX lateral con 4 hilos.
- Lavado articular, cierre de portales con agrafes e inmovilización con cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo durante 4-5 semanas. Puede retirarlo para aseo personal y para realizar ejercicios de flexo-extensión de codo así como pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Analgesia por elastómero prescrito por Servicio de Anestesia durante las primeras 24-48h. Continuar una vez retirado con Dexketoprofeno 25 mg v.o. 1/8 horas vía oral durante 4-5 días. Puede alternar con Metamizol caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 12-14 días
- Puede requerir reposo / ayuda domiciliaria
- Pedir cita con Servicio de RHB antes de marcharse de alta

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `hombro_balon` — CAH — Rotura masiva + balón subacromial

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + locorregional. Profilaxis ATB. Decúbito lateral ${DECUBITO}.
- CAH ---.
- Portales habituales
- Glenohumeral: PLB degenerado y deshilachado por lo que se realiza tenotomía, labrum bien, rotura subescapular tipo 2 de Lafosse. Se realiza reparación con 1 Iconix 2,3 (2 suturas tendón-hueso). Rotura supraespinoso grado 3 de Patte que se extiende a infraespinoso (rotura masiva).
- Subacromial: bursectomía, se localiza rotura supraespinoso. Tendón retraído hasta reborde glenoideo. Se realiza reparación infraespinoso con 1 arpón Peek-Zip 5,5 (2 suturas). Supraespinoso no reparable por lo que se coloca balón subacromial InSpace talla M.
- Lavado articular, cierre de portales con agrafes e inmovilización con cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo durante 4-5 semanas. Puede retirarlo para aseo personal y para realizar ejercicios de flexo-extensión de codo así como pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Analgesia por elastómero prescrito por Servicio de Anestesia durante las primeras 24-48h. Continuar una vez retirado con Dexketoprofeno 25 mg v.o. 1/8 horas vía oral durante 4-5 días. Puede alternar con Metamizol caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 12-14 días
- Puede requerir reposo / ayuda domiciliaria
- Pedir cita con Servicio de RHB antes de marcharse de alta

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `hombro_cah_luxac` — CAH — Luxación AC + TwinBridge (S&N)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia general e IOT. Profilaxis antibiótica con 2g de cefazolina.
- En posición de silla de playa.
- Portales artroscópicos AL + AM. Localizamos tendón conjunto, apófisis coracoides y disecamos hasta base.
- Miniabordaje longitudinal sobre tercio medio de clavícula.
- Fijación interna sistema TwinBridge (Smith and Nephew).
- Comprobamos adecuada reducción y colocación de material.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con grapas.
- Apósito y cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener brazo en cabestrillo, moviendo mano y codo como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar coloración y sensibilidad de la mano y los dedos.
- Evitar cargar peso sobre brazo intervenido hasta nuevo aviso y según plazos marcados.

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- IBUPROFENO 400 mg cada 8 horas vía oral añadido a lo anterior si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 48-72 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en 3-4 semanas para ${DOCTOR}, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

<a id="categoría-hombro_pthi"></a>

#### Prótesis Hombro (4 plantillas)

##### `hombro_pthi_aequalis` — PTHI inversa Aequalis (fracturas)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + bloqueo locorregional. Profilaxis ATB.
- Silla de playa. Abordaje deltopectoral.
- Colocación PTHI --- Aequalis Reversed (Tornier) de fracturas:
- Metaglena 25 + tornillos
- Glenosfera 36
- Vástago 11 cementado por déficit consola medial
- Bandeja humeral 6 mm
- Reducción comprobando adecuada estabilidad protésica y balance articular.
- Reinserción de tuberosidades según técnica descrita por Boileau aportando injerto autólogo de cabeza humeral a metáfisis.
- Lavado, hemostasia, drenaje aspirativo, cierre por planos, inmovilización con cabestrillo.
- Pido Rx y hemograma
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo durante 4 semanas. Puede retirar cabestrillo eventualmente para aseo personal y para realizar ejercicios de flexoextensión de codo y pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Enanplus 1 c/12h vía oral si dolor
- Nolotil caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h
- Tratamiento domiciliario habitual
- Puede requerir ayuda domiciliaria

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 14-15 días
- Gestionar cita con Servicio de RHB antes de marcharse de alta

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `hombro_pthi_ascend` — PTHI inversa Ascend Flex (omartrosis)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + bloqueo locorregional. Profilaxis ATB.
- Silla de playa. Abordaje deltopectoral. Tenodesis PLB a pectoral mayor. Desinserción subescapular con pastilla ósea.
- Colocación PTHI --- Ascend Flex (Stryker/Tornier):
- Metaglena 25 + tornillos
- Glenosfera 36
- Vástago 5B no cementado, bandeja humeral centrada
- Inserto humeral 6 mm
- Reducción comprobando adecuada estabilidad protésica y balance articular.
- Reinserción de subescapular.
- Lavado, hemostasia, drenaje aspirativo, cierre por planos, inmovilización con cabestrillo.
- Pido Rx y hemograma
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo durante 4 semanas. Puede retirar cabestrillo eventualmente para aseo personal y para realizar ejercicios de flexoextensión de codo y pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Enanplus 1 c/12h vía oral si dolor
- Nolotil caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h
- Tratamiento domiciliario habitual
- Puede requerir ayuda domiciliaria

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 14-15 días
- Gestionar cita con Servicio de RHB antes de marcharse de alta

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `hombro_pthi_biorsa` — PTHI inversa Perform 2+ con BioRSA

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + bloqueo locorregional. Profilaxis ATB.
- Silla de playa. Abordaje deltopectoral. Tenotomía PLB. Desinserción subescapular.
- Extracción BioRSA 36 10 mm.
- Colocación PTHI --- (Stryker/Tornier):
- Metaglena 25 + tornillos 38 + injerto BioRSA
- Glenosfera 36
- Vástago Perform 2+ no cementado
- Inserto humeral 0
- Reducción comprobando adecuada estabilidad protésica y balance articular.
- Reinserción de subescapular transósea.
- Lavado, hemostasia, drenaje aspirativo, cierre por planos, inmovilización con cabestrillo.
- Pido Rx y hemograma
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo durante 4 semanas. Puede retirar cabestrillo eventualmente para aseo personal y para realizar ejercicios de flexoextensión de codo y pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Enanplus 1 c/12h vía oral si dolor
- Nolotil caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h
- Tratamiento domiciliario habitual
- Puede requerir ayuda domiciliaria

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 14-15 días
- Gestionar cita con Servicio de RHB antes de marcharse de alta

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `hombro_pthi_revive` — Revisión PTHI — vástago Flex Revive

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + bloqueo locorregional. Profilaxis ATB.
- Silla de playa. Incisión sobre cicatriz previa. Abordaje deltopectoral. Desinserción subescapular y troquíter. Se libera subescapular y supraespinoso. Exéresis de tejido fibrótico previo que se manda a microbiología, así como muestras de interfase de cemento, y tejido blando de glena y canal endomedular.
- Colocación PTHI --- Glena Reversed 2 y vástago Flex Revive (Stryker/Tornier):
- Metaglena 29 + tornillos
- Glenosfera 39
- Fresado del canal hasta 15 y eliminación de osteofito en calcar. Colocación de Vástago Flex Revive nº 15 (vástago y cuerpo metafisario) no cementado (queda estable), bandeja humeral centrada 1,5
- Inserto humeral 9 mm
- Reducción comprobando adecuada estabilidad protésica y balance articular.
- Reinserción de subescapular y troquíter a prótesis y diáfisis con PDS 1.
- Lavado, hemostasia, drenaje aspirativo, cierre por planos, inmovilización con cabestrillo.
- Pido Rx y hemograma
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo durante 4 semanas. Puede retirar cabestrillo eventualmente para aseo personal y para realizar ejercicios de flexoextensión de codo y pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Enanplus 1 c/12h vía oral si dolor
- Nolotil caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h
- Tratamiento domiciliario habitual
- Puede requerir ayuda domiciliaria

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 14-15 días
- Gestionar cita con Servicio de RHB antes de marcharse de alta

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

<a id="categoría-hombro_tumor"></a>

#### Tumores / Partes Blandas (1 plantillas)

##### `hombro_elastofibroma` — Exéresis de elastofibroma dorsii

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. Decúbito prono.
- Abordaje paraescapular oblicuo.
- Apertura dorsal ancho, disección profunda, exéresis elastofibroma dorsii.
- Se envía pieza a AP.
- Hemostasia cuidadosa, lavado, drenaje aspirativo, cierre por planos.
- Apósito compresivo.
- No es CMA
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el miembro superior operado en cabestrillo 1 semana. Puede retirar cabestrillo eventualmente para aseo personal y para realizar ejercicios de flexoextensión de codo y pendulares
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Paracetamol 1 g v.o. /8h vía oral
- Nolotil caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h
- Tratamiento domiciliario habitual
- Puede requerir ayuda domiciliaria

Curas locales c/72h y retirada de puntos por ATS DE ZONA en 14-15 días
- Pedir cita para Sala de Curas en 5-7 días

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

<a id="categoría-codo"></a>

#### Codo (3 plantillas)

##### `codo_biceps_agudo` — Reinserción bíceps distal agudo (Arthrex)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. + locorregional. Profilaxis ATB. Isquemia preventiva. Mesa de mano.
- Abordaje anterior. Localización cabo tendinoso. Se referencia con cintas de alta resistencia (Arthrex).
- Reinserción en tuberosidad bicipital con sistema Biceps Button de Arthrex + tornillo interferencial (túnel ciego de 7 mm).
- Se retira isquemia, hemostasia, lavado y cierre por planos.
- Inmovilización con férula braquial.
- Alta CMA esta tarde si buena evolución.
- Pido Rx
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- FÉRULA BRAQUIAL 3 semanas. Mantener brazo elevado en cabestrillo
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Analgesia por elastómero prescrito por Servicio de Anestesia durante las primeras 24-48h. Continuar una vez retirado con Dexketoprofeno 25 mg v.o. 1/8 horas vía oral durante 4-5 días. Puede alternar con Metamizol caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h
- NO CURAR HASTA REVISIÓN EN SALA DE CURAS TRAUMATOLOGÍA EN 12-14 DÍAS SALVO INCIDENCIA CLÍNICA, debiendo recolocar férula (PEDIR CITA PARA SALA DE CURAS TRAUMATOLOGÍA)
- Pedir cita con Servicio de RHB antes de marcharse de alta

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `codo_biceps_cronico` — Reinserción bíceps distal crónico con plastia ST

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. Profilaxis ATB. Mesa de mano.
- 1ºT Extracción ST autólogo por posterior de MI. Grosor plastia 7 mm.
- 2ºT Abordaje anterior. Se referencia rama cutánea antebraquial. Reinserción de plastia en tuberosidad bicipital con sistema Biceps Button de Arthrex + tornillo interferencial (túnel ciego de 7 mm).
- Localización de muñón bicipital proximal, disección y movilización del mismo.
- Sutura T-T de plastia a muñón con suturas de alta resistencia Fiber-Wire.
- Hemostasia, lavado y cierre por planos.
- Inmovilización con férula braquial.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- FÉRULA BRAQUIAL 3 semanas. Mantener brazo elevado en cabestrillo
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Enanplus 75 mg v.o. 1/12 horas vía oral durante 4-5 días. Puede alternar con Metamizol caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h
- Enoxaparina Rovi 40 mg 1 iny. s.c c/24h 10 días
- NO CURAR HERIDA DEL BRAZO INTERVENIDO HASTA REVISIÓN EN SALA DE CURAS TRAUMATOLOGÍA EN 12-14 DÍAS SALVO INCIDENCIA CLÍNICA, debiendo recolocar férula (PEDIR CITA PARA SALA DE CURAS TRAUMATOLOGÍA)
- Curar pequeña herida de la pierna c/72h y retirar puntos en 10 días
- Requiere ayuda y reposo domiciliario
- Pedir cita con Servicio de RHB antes de marcharse de alta

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `codo_epicondilitis` — Cirugía de Nirschl (epicondilitis)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Anestesia gral. Supino. Isquemia preventiva. Mesa de mano.
- Técnica de Nirschl. Perforaciones con AK en epicóndilo.
- Lavado profuso y cierre por planos.
- Vendaje.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener brazo elevado las primeras 24-48h. Puede mover codo libremente sin realizar esfuerzos ni coger peso durante 3 semanas al menos
- Mover activamente los dedos de la extremidad operada
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Dexketoprofeno 25 mg v.o. 1/8 horas vía oral durante 4-5 días. Puede alternar con Metamizol caps. 1 c/8h si más dolor
- Omeprazol 20 mg v.o. 1 c/24h

Curas locales c/3-4 días y retirada de puntos por ATS-DUE de zona en 12-14 días según evolución

REVISIÓN
- Solicitar cita para revisión en 4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

<a id="categoría-ms"></a>

#### Mano y Antebrazo (10 plantillas)

##### `ms_stc` — Síndrome del túnel carpiano (STC)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- ISQUEMIA POR ELEVACIÓN EN RAÍZ BRAZO.
- ANESTESIA  LOCAL Y  SEDACIÓN.
- MINIINCISIÓN  LONGITUDINAL EN  EJE DEL  4º DE  UNOS 2 CM
- LIBERACIÓN  DEL  CANAL  DEL  CARPO MEDIANTE RETINACULOTOMÍA SEGÚN TÉCNICA DE RAIMONDI  CON  SECCIÓN DEL  LIGAMENTO  TRANSVERSO  DEL CARPO.
- SE  LIBERA  ISQUEMIA  Y  SE COAGULA  VASOS  SANGRANTES  CON  BIPOLAR.
- CIERRE DE PIEL  CON  MONOFILAMENTO.
- VENDAJE CORRECTOR.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la extremidad en alto (brazo en cabestrillo y/o pie en alto) durante las primeras 48 horas.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- METAMIZOL 575mg/ 8 horas vía oral/5 dias
- PARACETAMOL 1 g/vo/8h/7 dias
- Retirada de puntos por su enfermero/a de referencia en el centro de salud en 12-15 días.

Curas locales cada 48h en su Centro de Salud
- Una vez retirados los puntos masajear zona de cicatriz de manera enérgica y en círculos.
- Evitar coger peso y hacer fuerza con la mano intervenida durante 8 semanas.

REVISIÓN
- Solicitar cita para revisión en 4/6 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_tcg` — TCG Mano (quiste sinovial)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Bajo anestesia general, decúbito supino, isquemia de MS ${LADO_M}.
- Se realiza abordaje sobre tumoración.
- Exéresis de tumoración de diámetro aprox de 2 cm, consistencia gomosa, color parduzco y no adherido a planos profundos, compatible con tumor de células gigantes.
- Se manda muestra para estudio Anatomía Patológica.
- Lavado, hemostasia y cierre.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la extremidad en alto (brazo en cabestrillo) durante las primeras 48 horas.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Paracetamol 600 mg v.o. cada 8 horas durante 5 días.
- Metamizol 575 mg v.o. cada 8 horas durante 5 días.
- Realizar masajes sobre cicatriz una vez retirados los puntos.
- Retirada de puntos por su enfermero/a de referencia en el centro de salud en 12-15 días. Curas locales en su Centro de Salud cada 48h.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_dedo_resorte` — Dedo en resorte — apertura polea A1

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Bajo anestesia local y sedación, en decúbito supino, con manguito de isquemia en raíz de MS ${LADO_M}.
- Se realiza poleotomía tras incisión en cara volar base --- dedo.
- Lavado, hemostasia y cierre.
- Vendaje.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la mano elevada el mayor tiempo posible durante las primeras 48 horas.
- Mover activamente los dedos de la extremidad operada, según se le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral durante 5 días, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas durante 5 días.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando puntos de sutura en 12-15 días, salvo mejor criterio de enfermería de zona.
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma.
- Evitar coger peso y hacer fuerza con la mano intervenida durante 4 semanas desde la fecha de la intervención.

REVISIÓN
- Solicitar cita para revisión en 3-4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_dedo_resorte_tenolisis` — Dedo en resorte — tenolisis

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Bajo anestesia local, decúbito supino, isquemia de MS ${LADO_M}.
- Abordaje transversal sobre pliegue proximal de articulación MCF --- dedo mano ${LADO_F}.
- Apertura polea A1 comprobándose liberación completa de tendón FPL.
- Lavado, hemostasia y cierre.
Retirada de puntos por su enfermero/a de referencia en el centro de salud en 12-15 días. Curas locales en su Centro de Salud cada 48h
Solicitar cita para revisión en 4 semanas para ${DOCTOR}
Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Puede requerir ayuda domiciliaria

CURAS LOCALES
- Curas planas cada 48-72 horas.
```

##### `ms_seccion_tendon` — Sección tendón flexor mano

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Isquemia en raíz brazo.
- Anestesia general con mascarilla laríngea.
- Ampliación de la herida inicial a nivel del pliegue flexor de la IFP del dedo.
- Identificación de la sección completa del tendón flexor profundo y parcial de la bandeleta cubital del flexor superficial.
- Sutura del flexor profundo con doble marco de Kessler y puntos en corona.
- Sutura de la bandeleta superficial con dos puntos. Ambos con monofilamento reabsorbible.
- Lavado herida, se libera isquemia y coagulación vasos sangrantes con bipolar.
- Sutura piel con monofilamento.
- Férula de inmovilización.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la extremidad en alto (brazo en cabestrillo y/o pie en alto) durante las primeras 48 horas.
- Mover activamente los dedos de la mano  libres.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Puede requerir ayuda domiciliaria
- CIPROFLOXACINO  750 mg/ 12 h durante una semana
- METAMIZOL 575mg/ 8 horas vía oral
- PARACETAMOL 1 g/vo/8h
- Acudir a SALA DE CURAS DE  COT (GABINETE 7) para ver estado de herida y citar en función de la misma.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3 semanas para ${DOCTOR}
- Una vez retirados los puntos masajear zona de cicatriz de manera enérgica y en círculos.
- Evitar coger peso y hacer fuerza con la mano intervenida durante 8 semanas.

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_cerclaje_clavicula` — Weaver-Dunn / Fr clavícula distal — cerclaje

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Luxación acromioclavicular / fractura distal clavícula ${LADO_F}.
- Anestesia general e IOT. Profilaxis antibiótica con 2g de cefazolina.
- En posición de silla de playa.
- Abordaje directo sobre trazo de fractura, longitudinal a clavícula, reducción abierta.
- Lazada de PDS a través de dos orificios en clavícula y bajo base de coracoides.
- Lazada en 8 a través de orificios reduciendo fractura.
- Plastia con pastilla ósea de hemiligamento coracoacromial a clavícula distal.
- Comprobamos adecuada reducción.
- Lavado abundante con suero fisiológico.
- Cierre por planos con sutura reabsorbible, y piel con sutura intradérmica.
- Apósito y cabestrillo.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener brazo en cabestrillo, moviendo mano y codo como se le ha explicado.
- Realizar los ejercicios que su médico le ha explicado.
- Vigilar coloración y sensibilidad de la mano y los dedos.
- Evitar cargar peso sobre brazo intervenido hasta nuevo aviso y según plazos marcados.

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- IBUPROFENO 400 mg cada 8 horas vía oral añadido a lo anterior si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 48-72 horas, retirando grapas en 15-17 días, salvo mejor criterio de enfermería de zona.

REVISIÓN
- Solicitar cita para revisión en 3-4 semanas para ${DOCTOR}, para control evolutivo y radiológico.

SÍNTOMAS DE ALERTA
- Si aparece fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_dupuytren` — Dupuytren — fasciectomía

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Bajo anestesia regional y sedación, en decúbito supino, con manguito de isquemia en raíz de MS ${LADO_M}.
- Abordaje en zigzag sobre cordón fibroso --- radio.
- Escisión del mismo, comprobando extensión completa de articulaciones metacarpofalángica e interfalángicas.
- Lavado, hemostasia y cierre.
- Vendaje.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la mano elevada el mayor tiempo posible durante las primeras 48 horas.
- Mover activamente los dedos de la extremidad operada, según se le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.

MEDICACIÓN (según tarjeta sanitaria)
- METAMIZOL 575mg cada 8 horas vía oral durante 5 días, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas durante 5 días.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 24-48 horas, retirando puntos de sutura en 12-15 días, salvo mejor criterio de enfermería de zona.
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma.
- Evitar coger peso y hacer fuerza con la mano intervenida durante 4 semanas desde la fecha de la intervención.

REVISIÓN
- Solicitar cita para revisión en 3-4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_ganglion` — Ganglión mano — resección

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Bajo anestesia local y sedación, en decúbito supino, con manguito de isquemia en raíz de MS ${LADO_M}.
- Incisión en cara dorsal de mano.
- Resección de la lesión hasta punto de comunicación con articulación, y electrocoagulación del mismo.
- Lavado, hemostasia y cierre.
- Vendaje.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la mano elevada el mayor tiempo posible durante las primeras 48 horas.
- Mover activamente los dedos de la extremidad operada, según se le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- METAMIZOL 575mg cada 8 horas vía oral durante 5 días, que puede alternar con PARACETAMOL 1g/8h vía oral si precisa por dolor.
- OMEPRAZOL 20mg cada 24 horas durante 5 días.

CURAS LOCALES
- Realizar curas locales en el centro de salud cada 48-72 horas, retirando puntos de sutura en 12-15 días, salvo mejor criterio de enfermería de zona.
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma.

REVISIÓN
- Solicitar cita para revisión en 3-4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_infiltracion_tmct` — Infiltración TMTC-STT bajo escopia

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Infiltración bajo escopia TMTC-STT mano ${LADO_F} con AL+CE.
- Inmediata mejoría del dolor.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Reposo mano ${LADO_F} 24-48 horas.
- Mover activamente los dedos de la extremidad operada, según se le ha explicado.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Retirar apósito pasadas las 6-8 horas de la intervención.

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión en 3-4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

##### `ms_rizartrosis` — Rizartrosis — trapeciectomía + plastia Welby

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Bajo anestesia locorregional + sedación, decúbito supino, isquemia de MS ${LADO_M}.
- Abordaje dorsal de TMC primer dedo y técnica de Welby modificada.
- Identificación de rama sensitiva dorsal del nervio radial.
- Exéresis de trapecio, comprobando buen estado de superficie articular de escafoides y trapezoide e integridad de arteria radial.
- Se obtiene el hemitendón radial del FCR.
- Plastia con hemiFCR sobre APL y hemiFCR anclado en 2º MTC.
- Se quita la isquemia comprobando que no hay sangrado activo.
- Cierre por planos.
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener la extremidad en alto (brazo en cabestrillo) durante las primeras 48 horas.
- Mover activamente los dedos de la extremidad operada.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- ELASTÓMERO 48H. Acudir al centro de salud o al hospital para retirada pasadas las 48h. A partir de entonces comenzar con tratamiento oral:
- METAMIZOL 575mg/vo/8h/5 días
- PARACETAMOL 1g/vo/8h/5 días

Curas locales cada 48-72h. Retirada de puntos a partir de los 12-15 días.

REVISIÓN
- Solicitar cita para revisión en 4 semanas para ${DOCTOR}

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada acudirá a Urgencias.
```

<a id="región-pt"></a>

### Región: Pie y Tobillo

<a id="categoría-pt"></a>

#### Pie y Tobillo (5 plantillas)

##### `pt_antepie` — Antepié — SCARF/AKIN/Weil (Stryker)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica
- Isquemia preventiva de miembro inferior ${LADO_M}
- Abordaje medial sobre 1º radio
- Disección cuidadosa por planos, liberación de rama dorsal de nervio
- Osteotomía SCARF sobre M1, AKIN sobre F1, fijados con sendos tornillos FIXOS STRYKER
- Lavado profuso
- Comprobación adecuada colocación implantes y balance articular completo
- Cierre por planos
- Piel con reabsorbible/grapas
- Abordaje longitudinal intermetatarsiano para osteotomía de Weil triplanar sobre M2 fijado con tornillo TWISTOFF STRYKER
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener el pie elevado siempre que esté sentado
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos
- Caminar apoyando TODO EL PIE. Para ello, recomendamos comprar un zapato de postoperatorio (para apoyar todo el pie), de venta libre en ortopedias. Puede solicitar bastones en préstamo
- Estiramientos de gemelos e isquiotibiales
- Mantener vendaje 4-6 semanas
- Puede requerir ayuda domiciliaria
- Paracetamol 325 mg / Tramadol 37,5 mg cada 8h vía oral
- Metamizol 575 mg cada 8h alterno con lo anterior si precisa
- Omeprazol cada 24h
- Enoxaparina sc 40 mg cada 24h
- Cita en sala de curas de COT (Gabinete 7) en unos 3-5 días para valorar herida
- No es preciso retirar sutura. Puede ayudar a su caída frotando la herida durante el lavado a partir de la 3ª semana de la intervención
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma
- Debe evitar fumar hasta que la herida esté cicatrizada, no obstante, aconsejamos el abandono definitivo del tabaco si es usted fumador

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión con ${DOCTOR} en 4 semanas

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
```

##### `pt_pie_plano_osteo` — Pie Plano — Osteotomía (Koustogiannis + Evans + Cotton)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica
- Anestesia raquimedular
- Isquemia preventiva de miembro inferior ${LADO_M}
- Decúbito supino, abordaje lateral sobre calcáneo
- Osteotomía tipo Koustogiannis fijada con 2 tornillos ASNIS STRYKER de 6,5 mm / AUTOFIX STRYKER 6,5 mm
- Osteotomía de alargamiento de columna externa tipo Evans con cuña de aloinjerto fijada con tornillos ASNIS de 4 mm
- Osteotomía de apertura dorsal tipo Cotton sobre la base del 1º MTT con aloinjerto fijada con placa VARIAX STRYKER
- Comprobación por escopia adecuada colocación implantes y realineación del pie
- Lavado profuso
- Cierre por planos
- Piel con reabsorbible
- Vendaje algodonado
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pierna en alto y moviendo dedos y tobillo como se explica
- Puede ponerse frío local, nunca directamente sobre la piel, para el control de la inflamación
- Descarga de la pierna intervenida hasta la revisión en consulta. Puede solicitar muletas/silla de ruedas en préstamo
- Ibuprofeno 600 mg 1 comprimido cada 8 horas durante 5-7 días
- Paracetamol-Tramadol 325/37,5 mg 1 comprimido cada 8 horas alterno con lo anterior si precisa
- Enoxaparina 40 mg 1 inyección cada 24h durante 30 días
- Omeprazol 20 mg 1 comprimido cada 24 horas durante 30 días
- Precisa cuidados domiciliarios
- Cita en sala de curas de COT (Gabinete 7) en unos 3-5 días para valorar herida
- Debe evitar fumar hasta que la herida esté cicatrizada, no obstante, aconsejamos el abandono definitivo del tabaco si es usted fumador

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión con ${DOCTOR} en 4 semanas

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
- No es preciso retirar sutura. Puede ayudar a su caída frotando la herida durante el lavado a partir de la 3ª semana de la intervención
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma
```

##### `pt_pie_plano_artrodesis` — Pie Plano — Artrodesis subastragalina + talonavicular

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica
- Anestesia raquimedular
- Isquemia preventiva de miembro inferior ${LADO_M}
- Decúbito supino, abordaje medial
- Denudación de superficies articulares y artrodesis subastragalina + talonavicular
- Corrección de eje del retropié en el plano coronal y sagital
- Fijación con tornillos AUTOFIX 6,5 mm / ASNIS STRYKER 6,5 mm + tornillos AUTOFIX / ASNIS STRYKER 4 mm en "X"
- Comprobación por escopia adecuada colocación implantes y realineación del pie
- Lavado profuso
- Cierre por planos
- Piel con reabsorbible
- Vendaje algodonado
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pierna en alto y moviendo dedos y tobillo como se explica
- Puede ponerse frío local, nunca directamente sobre la piel, para el control de la inflamación
- Descarga de la pierna intervenida hasta la revisión en consulta. Puede solicitar muletas/silla de ruedas en préstamo
- Ibuprofeno 600 mg 1 comprimido cada 8 horas durante 5-7 días
- Paracetamol-Tramadol 325/37,5 mg 1 comprimido cada 8 horas alterno con lo anterior si precisa
- Enoxaparina 40 mg 1 inyección cada 24h durante 30 días
- Omeprazol 20 mg 1 comprimido cada 24 horas durante 30 días
- Precisa cuidados domiciliarios
- Cita en sala de curas de COT (Gabinete 7) en unos 3-5 días para valorar herida
- Debe evitar fumar hasta que la herida esté cicatrizada, no obstante, aconsejamos el abandono definitivo del tabaco si es usted fumador

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión con ${DOCTOR} en 4 semanas

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
- No es preciso retirar sutura. Puede ayudar a su caída frotando la herida durante el lavado a partir de la 3ª semana de la intervención
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma
```

##### `pt_pie_cavo_osteo` — Pie Cavo Varo — Osteotomía (Dwyer + Jones)

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica
- Anestesia raquimedular
- Isquemia preventiva de miembro inferior ${LADO_M}
- Decúbito supino, abordaje lateral sobre calcáneo
- Osteotomía tipo Dwyer + Koustogiannis inverso fijada con 2 tornillos ASNIS STRYKER de 6,5 mm / AUTOFIX STRYKER 6,5 mm
- Abordaje dorsomedial sobre primer radio
- Osteotomía de cierre dorsal tipo Jones sobre 1º MTT fijada con placa VARIAX STRYKER
- Comprobación por escopia adecuada colocación implantes y realineación del pie
- Lavado profuso
- Cierre por planos
- Piel con reabsorbible
- Vendaje algodonado
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pierna en alto y moviendo dedos y tobillo como se explica
- Puede ponerse frío local, nunca directamente sobre la piel, para el control de la inflamación
- Descarga de la pierna intervenida hasta la revisión en consulta. Puede solicitar muletas/silla de ruedas en préstamo
- Ibuprofeno 600 mg 1 comprimido cada 8 horas durante 5-7 días
- Paracetamol-Tramadol 325/37,5 mg 1 comprimido cada 8 horas alterno con lo anterior si precisa
- Enoxaparina 40 mg 1 inyección cada 24h durante 30 días
- Omeprazol 20 mg 1 comprimido cada 24 horas durante 30 días
- Precisa cuidados domiciliarios
- Cita en sala de curas de COT (Gabinete 7) en unos 3-5 días para valorar herida
- Debe evitar fumar hasta que la herida esté cicatrizada, no obstante, aconsejamos el abandono definitivo del tabaco si es usted fumador

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión con ${DOCTOR} en 4 semanas

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
- No es preciso retirar sutura. Puede ayudar a su caída frotando la herida durante el lavado a partir de la 3ª semana de la intervención
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma
```

##### `pt_pie_cavo_artrodesis` — Pie Cavo Varo — Artrodesis triple

**Nota Operatoria:**

```
IQ ${FECHA} (${DOCTOR}/${AYUDANTE})

- Profilaxis antibiótica
- Anestesia raquimedular
- Isquemia preventiva de miembro inferior ${LADO_M}
- Decúbito supino, abordaje medial y lateral
- Denudación de superficies articulares y artrodesis subastragalina + talonavicular + calcaneocuboidea
- Corrección de eje del retropié en el plano coronal y sagital
- Fijación con tornillos AUTOFIX 6,5 mm / ASNIS STRYKER 6,5 mm + tornillos AUTOFIX / ASNIS STRYKER 4 mm en "X" + placa VARIAX STRYKER / tornillos ASNIS / AUTOFIX 4 mm en calcaneocuboidea respectivamente
- Comprobación por escopia adecuada colocación implantes y realineación del pie
- Lavado profuso
- Cierre por planos
- Piel con reabsorbible
- Vendaje algodonado
```

**Tratamiento al Alta:**

```
CUIDADOS POSTOPERATORIOS
- Mantener pierna en alto y moviendo dedos y tobillo como se explica
- Puede ponerse frío local, nunca directamente sobre la piel, para el control de la inflamación
- Descarga de la pierna intervenida hasta la revisión en consulta. Puede solicitar muletas/silla de ruedas en préstamo
- Ibuprofeno 600 mg 1 comprimido cada 8 horas durante 5-7 días
- Paracetamol-Tramadol 325/37,5 mg 1 comprimido cada 8 horas alterno con lo anterior si precisa
- Enoxaparina 40 mg 1 inyección cada 24h durante 30 días
- Omeprazol 20 mg 1 comprimido cada 24 horas durante 30 días
- Precisa cuidados domiciliarios
- Cita en sala de curas de COT (Gabinete 7) en unos 3-5 días para valorar herida
- Debe evitar fumar hasta que la herida esté cicatrizada, no obstante, aconsejamos el abandono definitivo del tabaco si es usted fumador

CURAS LOCALES
- Curas planas cada 48-72 horas.

REVISIÓN
- Solicitar cita para revisión con ${DOCTOR} en 4 semanas

SÍNTOMAS DE ALERTA
- Si apareciera fiebre (>38º), dolor intenso que no se alivia con analgésicos, o alteraciones en la sensibilidad y/o la coloración de la extremidad operada se pondrá en contacto con su Centro de Salud en su horario de actividad o bien acudirá a Urgencias si ocurriera fuera de este horario
- No es preciso retirar sutura. Puede ayudar a su caída frotando la herida durante el lavado a partir de la 3ª semana de la intervención
- Una vez retirados los puntos, deberá masajear la zona de la cicatriz en círculos de forma enérgica, para evitar adherencias de la misma
```

<a id="módulo-urgencias"></a>

### Módulo: Urgencias

> Las plantillas de urgencias tienen una estructura diferente a las quirúrgicas. Cada plantilla genera tres secciones: **Anamnesis**, **Exploración** y **Plan** (conservador y/o quirúrgico). Las variables dinámicas son: `${COT}` (nombre del COT de guardia), `${ACUDO}` (Acudo/Acudimos según nº de COTs), `${PARTE}` (como parte/por orden), `${SEXO}` (Varón/Mujer), `${EDAD}` (edad), `${LADO}` (D/I).

<a id="categoría-urgencias"></a>

#### Urgencias (7 plantillas)

##### `urg_fx_edr` — Fx EDR (radio distal)

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${ACUDO} a paciente remitido desde puerta de urgencias para valoración y tratamiento de fractura de EDR ${LADO_M} ${PARTE}.

AP:
- NAMC
- No AP de interés

EA:
${SEXO} de ${EDAD} años que acude a urgencias por dolor e impotencia funcional de muñeca ${LADO_F} tras traumatismo.
```

**Exploración:**

```
EF:
- Tumefacción y deformidad en muñeca ${LADO_F} sin signos de sufrimiento de partes blandas. No equimosis ni flictenas.
- Dolor a la palpación y movilización de extremo distal de radio.
- Movilidad digital correcta dificultada por dolor sin signos de alteraciones NV.

Rx:
- Fx EDR ${LADO_M}.
```

**Plan (conservador):**

```
PLAN:
- Bajo bloqueo intrafocal con mepivacaína al 2%, procedo a reducción cerrada de fractura e inmovilización con yeso antebraquial cerrado.
- Rx de control ok.
- Explico plan terapéutico.

RECOMENDACIONES:
- Mantener mano en alto moviendo dedos.
- Ibuprofeno 400 mg/8 horas alternando con metamizol 575 mg/8h si dolor.
- Revisión en CCEE de COT (RUCOT) en 2 semanas con Rx previa.
```

**Plan (quirúrgico):**

```
PLAN:
- Curso analítica con perfil preoperatorio.
- Entrego CI que entiende, acepta, firma y traerá firmado el día de la intervención.
- Solicitará cita para consultas de Preanestesia en Admisión.
- Su caso se presentará en Sesión Clínica de Traumatología. Contactaremos con usted telefónicamente para comentar decisión tomada.

RECOMENDACIONES:
- Mantener mano en alto moviendo dedos.
- Ibuprofeno 400 mg/8 horas alternando con metamizol 575 mg/8h si dolor.
```

##### `urg_fx_5mtc` — Fx 5ºMTC (5º metacarpiano)

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${ACUDO} a paciente remitido desde puerta de urgencias para valoración y tratamiento de fractura de 5ºMTC ${LADO_M} ${PARTE}.

AP:
- NAMC
- No AP de interés

EA:
${SEXO} de ${EDAD} años que acude a urgencias por dolor e impotencia funcional de mano ${LADO_F} tras traumatismo.
```

**Exploración:**

```
EF:
- Tumefacción y deformidad en mano ${LADO_F} sin signos de sufrimiento de partes blandas.
- Dolor a la palpación del 5ºMTC.
- No signos de rotación del 5º dedo.
- Movilidad digital correcta.

Rx:
- Fx 5ºMTC ${LADO_M}.
```

**Plan (conservador):**

```
PLAN:
- Bajo bloqueo intrafocal con mepivacaína al 2%, procedo a reducción cerrada e inmovilización con yeso antebraquial cerrado incluyendo 4º-5º dedos.
- Rx de control ok.
- Explico plan terapéutico.

RECOMENDACIONES:
- Mantener mano en alto moviendo dedos libres.
- Ibuprofeno 400 mg/8 horas alternando con metamizol 575 mg/8h si dolor.
- Revisión en CCEE de COT (RUCOT) en 2 semanas con Rx previa.
```

##### `urg_fx_eph` — Fx EPH (húmero proximal)

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${ACUDO} a paciente remitido desde puerta de urgencias para valoración y tratamiento de fractura de húmero proximal ${LADO_M} ${PARTE}.

AP:
- NAMC
- No AP de interés

EA:
${SEXO} de ${EDAD} años que acude a urgencias por dolor e impotencia funcional de hombro ${LADO_M} tras traumatismo.
```

**Exploración:**

```
EF:
- Tumefacción en hombro ${LADO_M}.
- Dolor a la palpación y movilización.
- No signos de afectación neurovascular distal.

Rx:
- Fractura húmero proximal ${LADO_M}.
```

**Plan (conservador):**

```
PLAN:
- Inmovilización con cabestrillo interno + cinturón antirrotación.
- Explico plan terapéutico.

RECOMENDACIONES:
- Dormir semiincorporado.
- No apoyar codo en superficies.
- Mover activamente dedos y muñeca.
- Ibuprofeno 400 mg/8 horas alternando con metamizol 575 mg/8h si dolor.
- Revisión en CCEE de COT (RUCOT) en 2 semanas con Rx previa.
```

**Plan (quirúrgico):**

```
PLAN:
- Curso analítica con perfil preoperatorio.
- Entrego CI que entiende, acepta, firma y traerá firmado el día de la intervención.
- Solicitará cita para consultas de Preanestesia en Admisión.
- Su caso se presentará en Sesión Clínica de Traumatología. Contactaremos con usted telefónicamente para comentar decisión tomada.

RECOMENDACIONES:
- Inmovilización con cabestrillo interno + cinturón antirrotación.
- Dormir semiincorporado.
- No apoyar codo en superficies.
- Ibuprofeno 400 mg/8 horas alternando con metamizol 575 mg/8h si dolor.
```

##### `urg_fx_cadera` — Fx Cadera

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${ACUDO} a paciente remitido desde puerta de urgencias para valoración y tratamiento de fractura de cadera ${LADO_F} ${PARTE}.

AP:
- NAMC
- AP: ___

EA:
${SEXO} de ${EDAD} años que acude a urgencias por dolor inguinal e impotencia funcional de miembro inferior ${LADO_M} tras caída casual.
```

**Exploración:**

```
EF:
- Acortamiento y rotación externa de miembro inferior ${LADO_M}.
- Buen estado de partes blandas.
- Pulsos distales presentes. NV distal sin déficit.

Rx:
- Fractura de cadera ${LADO_F}.
```

**Plan (quirúrgico — siempre):**

```
PLAN:
- Entrego CI que entiende, acepta y firma.
- Curso analítica con perfil preoperatorio y pruebas cruzadas para reserva de 2 CH.
- Ingreso en observación a cargo de COT.
- Pendiente de programar para IQ.
```

##### `urg_fx_tobillo` — Fx Tobillo

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${ACUDO} a paciente remitido desde puerta de urgencias para valoración y tratamiento de fractura de tobillo ${LADO_M} ${PARTE}.

AP:
- NAMC
- AP: ___

EA:
${SEXO} de ${EDAD} años que acude a urgencias por dolor e impotencia funcional de tobillo ${LADO_M} tras traumatismo.
```

**Exploración:**

```
EF:
- Tumefacción moderada en tobillo ${LADO_M}.
- Posible deformidad.
- Deltoideo: ___
- Sindesmosis: ___
- Pulsos distales presentes. NV distal sin déficit.

Rx:
- Fractura de tobillo ${LADO_M}.
```

**Plan (conservador):**

```
RECOMENDACIONES:
- Pie en alto, mover activamente los dedos.
- NO apoyar.
- Paracetamol 1g/8h + Metamizol 575 mg/8h alterno si dolor.
- Enoxaparina 40 mg/24h sc.
- Omeprazol 20 mg/24h.
- Puede requerir ayuda domiciliaria.
- Revisión urgente en CCEE de COT en 1 semana (acudir media hora antes de cita para realizar Rx).
```

**Plan (quirúrgico):**

```
PLAN:
- Inmovilización con férula suropédica posterior.
- Entrego CI que entiende, acepta y firma.
- Curso analítica con perfil preoperatorio y pruebas cruzadas.
- Se cursa ingreso en planta.
```

##### `urg_fx_rotula` — Fx Rótula

> Con tipo (conservador / quirúrgico).

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

Interconsulta desde puerta de urgencias para valoración y tratamiento de fractura de rótula ${LADO_F}.

AP:
- NAMC
- AP: ___
- Situación basal: IABVD. Autonomía para la deambulación.

EA:
${SEXO} de ${EDAD} años que acude a urgencias por dolor e impotencia funcional en rodilla ${LADO_F} tras traumatismo casual.
```

**Exploración:**

```
EF:
- Tumefacción de rodilla ${LADO_F} moderada sin signos de sufrimiento de partes blandas.
- Sin derrame articular a tensión. Sin hematoma prerrotuliano.
- Dolor a la movilidad activa y pasiva de rodilla, así como a la palpación.
- Incapacidad para la extensión activa de rodilla.
- Incapacidad para mantenimiento isométrico de extensión.
- Movilidad distal conservada sin signos de alteraciones NV.

Rx:
- Fractura de rótula ${LADO_F}.
```

**Plan (conservador):**

```
PLAN:
- Inmovilización con férula inguinomaleolar posterior.
- Rx de control ok.
- Explico plan terapéutico.

TRATAMIENTO:
- Mantener el pie elevado siempre que esté sentado.
- Mover activamente los dedos de la extremidad.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Deambulación por domicilio con férula en extensión.
- Paracetamol 1g/8h alterno con Metamizol 575 mg/8h si dolor intenso.
- Omeprazol 20 mg/24h.
- Enoxaparina 40 mg/24h sc.
- Puede requerir ayuda domiciliaria.
- Revisión en CCEE de COT (RUCOT) en 2 semanas con Rx (acudir 30 minutos antes de cita para realización de radiografía).
```

**Plan (quirúrgico):**

```
PLAN:
- Inmovilización con férula inguinomaleolar posterior.
- Rx de control ok.
- Cursamos analítica con perfil preoperatorio.
- Entrego CI que entiende, acepta y firma.
- Solicitará cita para consultas de Preanestesia en Admisión.
- Su caso se presentará en Sesión Clínica de Traumatología. Contactaremos telefónicamente para comunicar decisión tomada.

TRATAMIENTO:
- Mantener el pie elevado siempre que esté sentado.
- Mover activamente los dedos de la extremidad.
- Vigilar la coloración y la sensibilidad de la extremidad y sus dedos.
- Paracetamol 1g/8h alterno con Metamizol 575 mg/8h si dolor intenso.
- Omeprazol 20 mg/24h.
- Enoxaparina 40 mg/24h sc.
- Puede requerir ayuda domiciliaria.
```

##### `urg_fx_vertebral` — Fx Vertebral

> Sin lateralidad (no aplica selector de lado).

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${ACUDO} a paciente tras interconsulta de puerta de urgencias por fractura vertebral ${PARTE}.
${SEXO} de ${EDAD} años que acude a urgencias por dolor en zona dorsolumbar de nueva aparición tras traumatismo en el día de hoy. No refiere pérdida de control de esfínteres. No refiere debilidad en MMII ni alteraciones en la sensibilidad.

AP:
- NAMC
- AP: ___
```

**Exploración:**

```
EF:
- Se explora en decúbito supino y lateral para palpación.
- Dolor a punta de dedo en línea media de zona dorsolumbar con irradiación a musculatura paravertebral.
- MMII: fuerza conservada 5/5 sin alteraciones en la sensibilidad.
- Sin clínica de afectación vascular.

Rx / TAC:
- Fractura vertebral ___ tipo ___.
```

**Plan (conservador):**

```
PLAN: manejo conservador.

RECOMENDACIONES:
- Reposo absoluto en cama durante 2 semanas. Puede levantarse solo para ir al baño e incorporarse para comer, pero siempre usando corsé recetado. El corsé no es necesario mientras esté tumbado en horizontal.
- Tras dichas 2 semanas, podrá realizar vida cama-sillón usando el corsé siempre que no esté acostado.
- Enoxaparina 40 mg/24h sc (1 inyección al día hasta revisión en consultas).
- Analgesia habitual si dolor. Si no dispone: Paracetamol 1g/8h alternando con Metamizol 575 mg/8h.
- SIGNOS DE ALARMA: pérdida de fuerza en miembros inferiores, alteraciones en la sensibilidad o pérdida de control de esfínteres → acudir a Urgencias.
- Revisión en CCEE de COT (RUCOT) en 1 mes con Rx (acudir 30 minutos antes de la cita para realización de la radiografía).
```

##### `urg_herida_tendon` — Herida con tendón

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${SEXO} de ${EDAD} años que acude a urgencias por herida inciso-contusa en ___ ${LADO_M}.
```

**Exploración:**

```
EF:
- Extensión completa.
- NV distal ok.

Bajo condiciones de asepsia y anestesia local con mepivacaína 2% se procede a exploración tendinosa, apreciándose sección parcial/total de tendón extensor/flexor ___.
- Sutura tipo marco Kessler con Monosyn 3.0.
- Sutura piel con Prolene 3.0.

Rx:
- ___.
```

**Plan (conservador):**

```
PLAN:
- Férula volar en extensión.
- Curas de la herida cada 48-72h por enfermería de su centro de salud.
- Retirada de puntos a criterio de atención primaria.

MEDICACIÓN:
- Paracetamol 1g/8h alterno con Metamizol 575 mg/8h si dolor intenso.
- Omeprazol 20 mg/24h.
- Amoxicilina/Clavulánico 875/125 mg cada 8 horas durante 10 días.

- Revisión en CCEE de COT (RUCOT) en 3 semanas.
```

##### `urg_lux_hombro` — Luxación Hombro

**Anamnesis:**

```
CONSULTA URGENCIAS COT
${FECHA_HOY}
${COT}

${ACUDO} a paciente remitido desde puerta de urgencias para valoración y tratamiento de luxación de hombro ${LADO_M} ${PARTE}.

AP:
- NAMC
- Episodios previos de luxación: ___

EA:
${SEXO} de ${EDAD} años que acude a urgencias por dolor e impotencia funcional de hombro ${LADO_M} tras traumatismo.
```

**Exploración:**

```
EF:
- Tumefacción y deformidad en hombro ${LADO_M} con aspecto en "charretera".
- Bloqueo de la rotación interna.
- Sensibilidad axilar conservada.
- Pulsos distales presentes. NV distal sin déficit.

Rx:
- Luxación glenohumeral ${LADO_F}.
```

**Plan (conservador):**

```
PLAN:
- Bajo analgesia iv, se procede a reducción cerrada mediante maniobra de tracción-contratracción.
- Rx post-reducción confirmatoria ok.
- Explico plan terapéutico.

RECOMENDACIONES:
- Cabestrillo tipo Sling: NO retirar.
- Ibuprofeno 400 mg/8 horas alternando con metamizol 575 mg/8h si dolor.
- Vigilar signos y síntomas.
- Revisión urgente en CCEE de COT en 3 semanas.
```

---

<a id="reglas-generales"></a>

## Reglas Generales

Ver [CLAUDE.md](./CLAUDE.md) para las reglas detalladas del proyecto.

Resumen:

1. **Header:** Toda plantilla empieza con `IQ ${FECHA} (${DOCTOR}/${AYUDANTE})`
2. **Formato:** Líneas con guión (`- `), título del procedimiento sin guión
3. **Revisión:** Siempre incluir `${DOCTOR}` en la línea de revisión
4. **Variables:** Usar `${FECHA}`, `${DOCTOR}`, `${AYUDANTE}` — nunca hardcodear
5. **Lateralidad:** Usar variables dinámicas (`${LADO_M}`, `${LADO_F}`, etc.) según género del sustantivo — nunca hardcodear
6. **Key:** Formato `snake_case` con prefijo de categoría
