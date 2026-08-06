# Guía Docente — Sesión 12: Escritura a múltiples voces

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivos `ejercicio_S12_voces.mscz`, `ejercicio_S12_coral.mscz` y `ejercicio_S12_limpieza.mscz` preparados por el docente  
**Referencia:** MuseScore Studio Handbook — Working with multiple voices, Brackets

---

## Objetivo de la sesión

Que el estudiante escriba dos líneas melódicamente independientes en un mismo pentagrama usando las voces 1 y 2 de MuseScore, gestione la dirección de plicas y la visibilidad de silencios, intercambie y reasigne voces correctamente, resuelva problemas de colisiones visuales en texturas polifónicas, y comprenda la diferencia conceptual entre voces (capas dentro de un pentagrama) y corchetes/llaves (agrupación visual entre pentagramas).

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S11 + pregunta disparadora: ¿cómo se escribe una fuga en un solo pentagrama? |
| **Desarrollo** | 30 min | Demostración: voces 1–4, colores, plicas, silencios, intercambio, corchetes y llaves |
| **Práctica** | 65 min | Piano a dos voces → coral contrapuntístico → limpieza de errores → reflexión sobre agrupación |
| **Cierre** | 15 min | Revisión por parejas, puesta en común, entrega |

---

## 1. Apertura — Revisión y activación

### Materiales
- Proyector con MuseScore Studio abierto.
- Los archivos `ejercicio_S12_voces.mscz`, `ejercicio_S12_coral.mscz` y `ejercicio_S12_limpieza.mscz` publicados en Classroom **antes de la clase**.

### Dinámica

1. **Revisión rápida de S11** (5 min):
   - ¿Lograron insertar correctamente las líneas de 8va sin dejar notas fuera?
   - ¿El pedal de piano: levantaron el pedal en los cambios de armonía?
   - ¿Las comas de respiración en el cuarteto de vientos: estaban en lugares lógicos?
   - ¿Recuerdan cuáles líneas afectan la reproducción y cuáles son solo visuales?

2. **Preguntas disparadoras** (5 min):
   - Proyectar un pentagrama con dos líneas melódicas independientes (ej. melodía + bajo). Preguntar: "¿Cuántas líneas melódicas ven aquí? ¿Cómo harían para escribir esto en MuseScore si todo está en el MISMO pentagrama?"
   - Mostrar un compás donde una nota negra en la parte superior suena simultáneamente con dos corcheas en la parte inferior. Preguntar: "¿Esto es un acorde o son dos líneas independientes? ¿Cómo lo diferencian visualmente?" (Las plicas: una hacia arriba, otra hacia abajo.)
   - Preguntar: "¿Alguna vez vieron una partitura de guitarra clásica o de un coral de Bach donde hay dos melodías en el mismo pentagrama? ¿Cómo saben cuál es cuál?"
   - Mostrar los botones de selección de voz (1, 2, 3, 4) en la barra de herramientas. Preguntar: "¿Para qué creen que sirven estos números?"

---

## 2. Desarrollo — Teoría guiada

### Secuencia sugerida

1. **Concepto de voces** (5 min). Proyectar un pentagrama vacío:
   - Explicar que MuseScore permite **hasta 4 voces independientes** por pentagrama. Cada voz es una "capa" que tiene sus propias notas, silencios, plicas y articulaciones.
   - "Piensen en capas de dibujo en Photoshop o GIMP: cada capa tiene su contenido, podés editarla por separado, pero al final se ven todas juntas."
   - Mostrar los colores de edición: "Durante la edición, la Voz 1 se ve azul, la Voz 2 verde, la Voz 3 naranja y la Voz 4 violeta. Estos colores NO se imprimen. Son solo para que no te pierdas."
   - Preguntar: "¿Cuántas voces creen que necesitan el 99% de las partituras?" (Respuesta: 1 o 2. Las voces 3 y 4 son para casos muy específicos.)

2. **Escritura a dos voces paso a paso** (8 min). Demostración práctica:
   - Activar modo de ingreso (`N`), seleccionar **Voz 1**, escribir una melodía simple en Do mayor (4 compases).
   - "Ahora quiero agregar una segunda línea debajo de esta melodía."
   - Volver al inicio, seleccionar **Voz 2**, escribir una línea de contrapunto.
   - **Momento de revelación**: mostrar cómo las plicas de la Voz 1 quedan hacia arriba y las de la Voz 2 hacia abajo automáticamente.
   - Señalar los silencios: donde la Voz 1 calla y la Voz 2 suena, aparece un silencio en la Voz 1. Y viceversa.
   - Mostrar cómo ocultar un silencio redundante: seleccionarlo, presionar `V`. El silencio se vuelve gris (invisible en el resultado final).
   - Preguntar: "Si en este tiempo suena la Voz 1, ¿necesito que se vea el silencio de la Voz 2?" (Generalmente no. El silencio de la voz complementaria es redundante.)

3. **Dirección de plicas y colisiones** (5 min). Sobre el ejemplo anterior:
   - Forzar la dirección de plica de una nota: seleccionar, panel Propiedades → Dirección de la plica → Arriba o Abajo.
   - Mostrar un caso donde las plicas automáticas colisionan con cabezas de la otra voz. "MuseScore suele manejar esto bien, pero a veces hay que ayudar."
   - Demostrar cómo ajustar el desplazamiento horizontal de una nota (panel Propiedades → Desplazamiento X) para evitar colisiones en casos extremos.
   - Preguntar: "¿Qué pasa si dos notas de diferente voz ocupan exactamente la misma altura y el mismo tiempo?" (MuseScore las dibuja con cabezas ligeramente desplazadas. Si la duración es diferente —ej. negra en Voz 1 y blanca en Voz 2— las cabezas se ven claramente separadas.)

4. **Gestión de voces: intercambiar y mover** (5 min). Sobre un ejemplo preparado:
   - "Supongamos que escribí toda la melodía principal en Voz 2 por error. No necesito borrar y reescribir."
   - Seleccionar el rango → **Herramientas → Voces → Intercambiar voz 1 y voz 2**. "Magia: la Voz 1 ahora tiene lo que estaba en Voz 2 y viceversa."
   - "¿Y si solo quiero mover ALGUNAS notas, no todo?" Seleccionar las notas específicas → **Herramientas → Voces → Mover a voz 2** (o `Ctrl + Alt + 2`).
   - Preguntar: "¿Cuándo usarían 'intercambiar' y cuándo 'mover'?" (Intercambiar: todo el contenido de dos voces. Mover: notas seleccionadas a otra voz.)

5. **Corchetes y llaves: agrupación de pentagramas** (5 min). Mostrar dos tipos de agrupación:
   - **Llave `{`**: une pentagramas de un MISMO instrumento (piano, arpa, órgano). Conecta las barras de compás formando el "gran pentagrama".
   - **Corchete `[`**: agrupa instrumentos de la MISMA familia (todos los violines, todas las flautas). No conecta las barras de compás.
   - Preguntar: "¿Por qué el cuarteto de cuerdas usa corchete y el piano usa llave?" (El cuarteto son 4 instrumentos distintos. El piano es UN solo instrumento con dos pentagramas.)
   - Preguntar: "¿Los corchetes y llaves afectan la reproducción?" (NO. Son puramente visuales. No tienen nada que ver con las voces.)
   - **Énfasis**: "No confundan voces con pentagramas. Voces = capas DENTRO de un pentagrama. Corchetes/llaves = agrupación ENTRE pentagramas."

6. **Voces 3 y 4: cuándo usarlas** (2 min):
   - Mostrar un caso donde realmente se justifican 3 voces: coral a 3 partes en un pentagrama.
   - "Para el 95% de lo que van a escribir en este curso, con Voz 1 y Voz 2 es suficiente. Las voces 3 y 4 son para contextos muy especializados. Si están usando la Voz 3, pregúntense: ¿no será mejor separar esto en otro pentagrama?"

---

## 3. Práctica — Escritura a múltiples voces

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S12 — Escritura a múltiples voces

**Material**: el docente proporciona tres archivos:

1. **`ejercicio_S12_voces.mscz`**: Partitura para piano (gran pentagrama) en Do mayor, 4/4, 16 compases.
   - **Pentagrama superior (mano derecha), compases 1–8**: melodía monofónica en Voz 1. Debe ser simple pero con suficiente variedad (negras, corcheas, alguna blanca, silencios) para que una segunda voz por debajo tenga sentido. Ámbito: Do₄–Sol₅. Sin alteraciones fuera de la escala.
   - **Pentagrama inferior (mano izquierda), compases 1–8**: bajo simple en Voz 1 en figuras largas (blancas y redondas) para que una segunda voz rítmica encima tenga espacio. Ámbito: Do₂–Do₃.
   - **Compases 9–16**: completamente vacíos en ambos pentagramas. El estudiante compondrá una sección nueva con textura polifónica.
   - Sin dinámicas, sin articulaciones (el foco total es la escritura a voces).

2. **`ejercicio_S12_coral.mscz`**: Partitura para voz (un solo pentagrama) en Fa mayor, 3/4, 8 compases.
   - Melodía de estilo coral (notas predominantemente blancas y negras con puntillo) en Voz 1. Movimiento diatónico con algún salto de tercera o cuarta. Sin alteraciones accidentales más allá del Si♭ de la armadura.
   - La melodía debe dejar espacio armónico para una segunda voz: evitar ámbitos demasiado extremos y mantener las notas en un registro medio (Do₄–Fa₅).
   - El archivo se entrega con solo la Voz 1 escrita.

3. **`ejercicio_S12_limpieza.mscz`**: Partitura para guitarra (un solo pentagrama) en La menor, 4/4, 12 compases.
   - **Errores intencionales que el docente debe incluir** (distribuidos en al menos 8 lugares diferentes):
     - Al menos 3 compases donde las notas de la melodía principal están en Voz 2 y deberían estar en Voz 1 (o viceversa).
     - Al menos 2 compases con silencios visibles redundantes que deberían ocultarse.
     - Al menos 1 compás con dirección de plicas inconsistente (Voz 1 con plicas hacia abajo, Voz 2 hacia arriba).
     - Al menos 2 compases con colisiones visuales (notas demasiado juntas entre voces, sin desplazamiento).
     - Algún compás con una nota en la voz equivocada (ej. una nota suelta que rompe la línea y claramente pertenece a la otra voz).
   - El archivo debe tener UNA sola voz visible a simple vista (la Voz 2 puede estar "escondida"). Incluir un pentagrama aparte o un texto de referencia indicando cómo DEBERÍA verse (no entregar esto al estudiante, solo al docente como guía de corrección).

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Agregar Voz 2 al pentagrama superior del piano (paralelismo armónico).
2. Agregar Voz 2 al pentagrama inferior del piano (acompañamiento rítmico).
3. Componer 8 compases polifónicos originales (c.9–16).
4. Añadir Voz 2 contrapuntística al coral.
5. Detectar y corregir ≥8 errores en el ejercicio de limpieza, documentándolos.
6. Reflexionar sobre la diferencia entre corchetes y llaves.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Dos voces en pentagrama superior | Voz 2 añadida con paralelismo correcto; plicas abajo; silencios redundantes ocultos; duraciones completas | Voz 2 presente pero con plicas incorrectas o silencios sin ocultar | Sin Voz 2 o graves errores de notación |
| Dos voces en pentagrama inferior | Voz 2 añadida con ritmo independiente del bajo; plicas arriba; silencios gestionados | Voz 2 sin independencia rítmica o plicas invertidas | Sin Voz 2 |
| Composición original (c.9–16) | Ambos pentagramas con dos voces originales; independencia rítmica y melódica; coherencia musical | Solo un pentagrama polifónico o poca independencia entre voces | Composición incompleta o completamente monofónica |
| Coral a dos voces | Voz 2 contrapuntística con intervalos consonantes y alguna nota de paso; sin colisiones ni silencios problemáticos | Voz 2 añadida pero con colisiones, silencios sucios o intervalos extraños | Sin Voz 2 o errores graves (choques de segundas, unísonos forzados) |
| Limpieza de voces | ≥8 errores correctamente identificados, corregidos y documentados; versión final limpia | 5–7 errores corregidos o documentación incompleta | <5 errores o sin documentación |
| Corchetes y llaves | Respuestas correctas y completas; demuestra comprensión de la diferencia conceptual | Respuesta parcialmente correcta (1 de 2) | Respuesta incorrecta o ausente |

---

## 4. Cierre — Dos líneas, un pentagrama

### Revisión por parejas (8 min)

Cada estudiante intercambia archivos con un compañero:
- Abre el archivo de piano del compañero. Escucha la composición de los compases 9–16: "¿Se distinguen las dos voces en cada mano? ¿Suena como una textura polifónica o como acordes?"
- Revisa los silencios: "¿Hay silencios visibles que sobran? ¿Todas las voces completan las duraciones de los compases?"
- En el coral: "¿La Voz 2 complementa la melodía o choca con ella? ¿Hay colisiones o segundas incómodas?"
- En el archivo de limpieza del compañero: "¿Encontró errores que vos no viste? ¿Coinciden en las correcciones?"

### Puesta en común (7 min)

Preguntas para guiar la discusión:
- "¿Qué fue más difícil: escribir la segunda voz desde cero o corregir los errores del archivo de limpieza?" (Esperado: corregir errores ajenos obliga a leer la partitura con más atención que escribir desde cero. Es una habilidad de edición profesional.)
- "¿En qué se diferencia una textura de 'melodía con acordes' de una textura de 'dos voces independientes'?" (En la melodía con acordes, el ritmo de las notas es el mismo en todas las voces. En dos voces independientes, cada voz tiene su propio ritmo y línea melódica.)
- "¿Cuándo conviene usar 2 voces en un pentagrama y cuándo conviene usar 2 pentagramas?" (Dos voces cuando es el MISMO instrumento con dos líneas cercanas en ámbito. Dos pentagramas cuando son instrumentos distintos o los ámbitos están muy separados.)
- "¿Alguien usó la Voz 3 o la Voz 4? ¿En qué situación?" (Probablemente nadie o muy pocos. Si alguien lo hizo, pedir que explique el contexto y discutir si era realmente necesario.)
- "¿Qué errores fueron los más difíciles de detectar en la limpieza?" (Esperado: las notas en la voz equivocada son difíciles de ver sin los colores de voz activados. Las colisiones visuales pueden ser subjetivas.)

### Resumen del docente (5 min)

1. Las voces son una de las herramientas más potentes y peor comprendidas de MuseScore. No son una curiosidad técnica: son la forma de escribir **música polifónica real** en un pentagrama.
2. La diferencia entre un acorde y dos voces es la **independencia rítmica**. Si todas las notas suenan al mismo tiempo, es un acorde (una sola voz). Si cada línea tiene su propio ritmo, necesitás voces separadas.
3. La gestión de **plicas y silencios** es lo que separa una partitura amateur de una profesional. Una partitura con plicas inconsistentes o silencios innecesarios grita "principiante". Afortunadamente, MuseScore automatiza la mayor parte, pero siempre hay que revisar.
4. Los **colores de edición** son tu mejor amigo al trabajar con voces. Si desactivás los colores (`Ver → Mostrar → Colores de voz`), distinguir la Voz 1 de la Voz 2 es casi imposible. Activá los colores siempre que estés editando voces.
5. **Voces ≠ Pentagramas ≠ Corchetes**. No confundir: voces son capas dentro de un pentagrama, corchetes agrupan pentagramas visualmente, y separar en pentagramas distintos es una decisión de diseño editorial. Cada herramienta tiene su propósito.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| El estudiante escribe la Voz 2 sin seleccionar el botón de Voz 2 y las notas van a la Voz 1 | Error MUY común. Las notas siempre van a la voz activa. Recordar: seleccionar la voz ANTES de escribir. Si ya escribió, usar Herramientas → Voces → Mover a voz 2. |
| Las plicas de la Voz 2 apuntan hacia arriba en vez de hacia abajo | Seleccionar las notas afectadas → panel Propiedades → Dirección de la plica → Abajo. O revisar si las notas están realmente en Voz 2 (a veces el estudiante piensa que están en Voz 2 pero en realidad están en Voz 1, y por eso las plicas van hacia arriba). |
| Los silencios de la Voz 2 tapan notas de la Voz 1 o viceversa | Enseñar a ocultar silencios con `V`. Mostrar que el silencio se vuelve gris (oculto). Recalcar que ocultar no es eliminar: la duración del compás sigue siendo correcta. |
| El estudiante no logra que las duraciones de la Voz 2 "cuadren" en el compás | Cada voz debe completar el compás de forma independiente. Si el compás es 4/4, la Voz 2 debe sumar 4 tiempos. Revisar que no falten silencios. MuseScore marca los compases incompletos con un pequeño signo `+` en la barra de estado. |
| Las notas de dos voces diferentes se superponen visualmente | Si son UNÍSONOS (misma altura y ritmo), es correcto. Si son notas diferentes en el mismo tiempo pero muy cercanas, MuseScore las desplaza automáticamente. Si no lo hace, ajustar manualmente con Propiedades → Desplazamiento X. Si colisionan una cabeza de nota con una plica, ajustar la plica. |
| El coral a dos voces resulta "feo" armónicamente (intervalos disonantes) | El estudiante puede no tener conocimientos de armonía. El objetivo de esta actividad NO es la corrección armónica sino la técnica de notación a dos voces. El docente puede sugerir "buscá terceras y sextas, evitá segundas y séptimas" como guía práctica rápida, pero no penalizar elecciones armónicas si no se ha enseñado armonía. |
| En la limpieza, el estudiante no encuentra los errores porque tiene los colores de voz desactivados | Recordar activar los colores de voz (por defecto están activados, pero si alguien los desactivó, no verá los colores azul/verde). Si el estudiante trabaja en una versión antigua de MuseScore, los colores pueden verse diferentes o estar desactivados por defecto. |
| El estudiante confunde "mover notas a otra voz" con "cambiar la dirección de plica" | No es lo mismo. Una nota en Voz 1 con plica hacia abajo sigue siendo Voz 1 (sigue teniendo el mismo "canal" de edición). Mover a Voz 2 la convierte en una nota independiente que se edita por separado. La dirección de plica es una propiedad visual; la asignación de voz es una propiedad estructural. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Working with multiple voices](https://handbook.musescore.org/basics/working-with-multiple-voices.md)
- [MuseScore Studio Handbook — Brackets](https://handbook.musescore.org/notation/brackets.md)
- **Preparación del archivo `ejercicio_S12_voces.mscz`**: crear partitura para piano en Do mayor, 4/4, 16 compases. Pentagrama superior: melodía en Voz 1, c.1–8, diatónica, variedad rítmica (negras, corcheas). Pentagrama inferior: bajo en Voz 1, c.1–8, figuras largas (blancas, redondas). c.9–16 vacíos. Sin dinámicas ni articulaciones. La melodía debe ser simple, casi "infantil", porque el estudiante va a duplicarla a distancia de tercera/sexta en Voz 2.
- **Preparación del archivo `ejercicio_S12_coral.mscz`**: crear partitura para voz (1 pentagrama) en Fa mayor, 3/4, 8 compases. Melodía en Voz 1 con carácter de coral (blancas con puntillo, negras, mínimas). Movimiento por grados conjuntos con algún salto. Registro medio (Do₄–Fa₅). Dejar suficiente "aire" entre notas para que la Voz 2 tenga espacio. Sin letra (la letra se verá en sesiones posteriores).
- **Preparación del archivo `ejercicio_S12_limpieza.mscz`**: la preparación de este archivo es la más laboriosa. El docente debe escribir una pieza CORRECTA primero (en La menor, 4/4, 12 compases, para guitarra, con textura a dos voces correcta y limpia). Luego, sobre una copia, introducir deliberadamente los errores listados en la sección de práctica. Es importante que los errores sean sutiles pero detectables: una nota en la voz equivocada que "rompe" la línea melódica, un silencio visible donde claramente sobra, plicas inconsistentes. El docente debe guardar la versión correcta como referencia para evaluar las entregas.
- Dato curioso: la notación polifónica en un solo pentagrama fue una innovación del Renacimiento. Antes, la música vocal se escribía en "libros de coro" donde cada voz tenía su propio pentagrama en páginas separadas (o en diferentes cuadrantes de una misma página doble). La idea de superponer dos voces en un mismo pentagrama usando plicas opuestas se desarrolló gradualmente durante los siglos XVI y XVII, y hoy es el estándar para música de teclado, guitarra y reducciones orquestales.
- Dato curioso: en MuseScore, las voces 1 y 2 tienen comportamientos de reproducción ligeramente diferentes para dinámicas y articulaciones: por defecto, una dinámica aplicada a la Voz 1 no afecta a la Voz 2. Esto permite controlar la expresión de cada línea de forma independiente, lo cual es fundamental en texturas contrapuntísticas.
- Ejercicio opcional de ampliación: proporcionar una invención a dos voces de Bach para que los estudiantes la transcriban en MuseScore usando Voces 1 y 2. Es un desafío exigente que integra lectura de partitura polifónica con dominio técnico de voces. Recomendado para estudiantes avanzados o como actividad de cierre de unidad.

---

*Guía docente — Tecnología Musical I | Sesión 12*
