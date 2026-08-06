# Guía Docente — Sesión 13: Repeticiones, voltas y saltos de navegación

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivos `ejercicio_S13_repeticiones.mscz`, `ejercicio_S13_navegacion.mscz` y `ejercicio_S13_barras.mscz` preparados por el docente  
**Referencia:** MuseScore Studio Handbook — Repeats and jumps, Voltas, Barlines

---

## Objetivo de la sesión

Que el estudiante inserte barras de repetición y voltas para estructurar secciones con finales alternativos, configure una navegación D.S. al Coda funcional con todos sus elementos (segno, To Coda, Coda, D.S.), corrija tipos de barras de compás según su función musical (doble, final, repetición), y diseñe un mapa de navegación propio integrando repeticiones, voltas y saltos en una estructura coherente.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S12 + pregunta disparadora: ¿cuántas veces tocamos la misma sección? |
| **Desarrollo** | 30 min | Demostración: barras de repetición → voltas → D.C./D.S. → Fine/Coda → barras especiales |
| **Práctica** | 65 min | Repeticiones y voltas en piano → D.S. al Coda en cuarteto → corrección de barras → Coda propia |
| **Cierre** | 15 min | Revisión por parejas, puesta en común, entrega |

---

## 1. Apertura — Revisión y activación

### Materiales
- Proyector con MuseScore Studio abierto.
- Los archivos `ejercicio_S13_repeticiones.mscz`, `ejercicio_S13_navegacion.mscz` y `ejercicio_S13_barras.mscz` publicados en Classroom **antes de la clase**.

### Dinámica

1. **Revisión rápida de S12** (5 min):
   - ¿Lograron escribir a dos voces sin que las plicas se vuelvan locas?
   - ¿Encontraron el error más difícil en el archivo de limpieza? ¿Cuál era?
   - ¿Recuerdan la diferencia entre corchetes y llaves? ¿Y entre voces y pentagramas?

2. **Preguntas disparadoras** (5 min):
   - Proyectar una partitura breve (8 compases) que termine con barra de fin de repetición. Preguntar: "Si tocamos esto en MuseScore, ¿qué va a pasar cuando llegue al final?" (Vuelve al inicio o al inicio de repetición.)
   - Proyectar la MISMA partitura pero ahora con dos casillas de volta. "¿Qué cambió ahora? ¿Cuántas veces se toca esta sección? ¿Los dos finales son iguales?"
   - Mostrar una partitura con un D.C. al Fine. Preguntar: "¿Qué significa D.C.? ¿Qué significa Fine? ¿En qué orden se toca esta pieza?"
   - Mostrar una partitura de musical o de banda con marcas como 𝄋 (segno) y 𝄌 (coda). Preguntar: "¿Alguna vez vieron estos símbolos? ¿Qué creen que significan? ¿Son lo mismo que las marcas de ensayo?"

---

## 2. Desarrollo — Teoría guiada

### Secuencia sugerida

1. **Barras de repetición** (5 min). Sobre una partitura de piano proyectada:
   - Mostrar las barras de inicio de repetición y fin de repetición en la paleta **Barras de compás**. "Estas dos barras forman un sándwich: todo lo que está adentro se toca dos veces."
   - Insertar inicio de repetición en el compás 1: seleccionar la barra, arrastrar la barra de inicio desde la paleta.
   - Insertar fin de repetición en el compás 8: mismo procedimiento.
   - Reproducir: la sección se toca dos veces automáticamente.
   - Preguntar: "¿Qué pasa si SOLO pongo el fin de repetición y no el inicio?" (MuseScore asume que la repetición empieza desde el principio de la pieza. Es válido pero puede ser confuso en partituras largas.)
   - Mostrar la barra **fin-inicio** (puntos a ambos lados): "Esto es eficiente: cierra la repetición de la sección anterior Y abre la repetición de la siguiente."

2. **Voltas: primera y segunda vez** (8 min). Sobre la misma partitura:
   - Extender la pieza: después del compás 8, agregar un final A (c.9–12) y un final B (c.13–16).
   - Preguntar: "¿Cómo le digo a MuseScore que la primera vez toque los compases 9–12 y la segunda vez los compases 13–16?"
   - Insertar la **volta 1**: seleccionar compases 9–12 → paleta **Repeticiones y saltos** → arrastrar la volta 1.
   - **Momento crítico**: "La volta 1 DEBE terminar con una barra de fin de repetición. Si no, MuseScore no entiende que tiene que repetir." Mostrar qué pasa si la volta termina con barra simple: no hay repetición.
   - Insertar la **volta 2**: seleccionar compases 13–16 → arrastrar volta 2. "Esta NO necesita barra de repetición al final porque después de la segunda vez, la pieza continúa normalmente."
   - Reproducir: primera pasada → volta 1 → repetir → saltar volta 1 → volta 2.
   - Mostrar el panel **Propiedades → Lista de repetición**. Explicar que se puede configurar para patrones complejos: `1,3` para primera y tercera vez, etc.
   - Preguntar: "¿Podría tener una volta 3?" (Sí, si la sección se repite 3 veces con 3 finales diferentes. Poco común pero posible.)

3. **D.C. al Fine y D.S. al Fine** (7 min). Sobre una partitura nueva con estructura A-B-A:
   - "Las barras de repetición son para secciones contiguas. ¿Qué pasa si quiero repetir una sección que NO está al lado?" → Presentar D.C. (Da Capo) y D.S. (Dal Segno).
   - Insertar un **Fine** al final de la sección A (compás 8): paleta **Repeticiones y saltos** → arrastrar Fine sobre la barra del compás 8.
   - Insertar un **D.C. al Fine** al final de la sección B (compás 24): paleta → arrastrar D.C. al Fine.
   - Reproducir: A → B → volver al principio → A (hasta Fine) → terminar.
   - Preguntar: "¿Qué pasa si pongo Fine pero NO pongo D.C.? ¿MuseScore se detiene en el Fine la primera vez?" (SÍ. El Fine es una parada INCONDICIONAL. Sin un D.C. o D.S. que "reactive" la ejecución, MuseScore se detiene en el primer Fine que encuentra.)
   - Reemplazar con D.S.: insertar un **segno** (𝄋) al inicio de A, cambiar D.C. por **D.S. al Fine**. Reproducir: B → D.S. → volver al segno → A → Fine.
   - Preguntar: "¿En qué se diferencia D.C. de D.S. en la práctica?" (D.C. siempre vuelve al principio. D.S. vuelve al segno, que puede estar en cualquier parte de la pieza. D.S. es más flexible.)

4. **D.S. al Coda: la estructura completa** (5 min). Sobre una partitura con más secciones:
   - Estructura: Introducción → Tema (con segno) → Desarrollo → Coda.
   - Insertar **segno** al inicio del Tema.
   - Insertar **To Coda** al final del Desarrollo.
   - Insertar **D.S. al Coda** al final del Tema (esto fuerza que el Tema se toque dos veces: una normal, y otra después del D.S.).
   - Insertar **Coda** al inicio de los compases finales (la sección Coda).
   - Reproducir el orden completo: Intro → Tema (hasta D.S. al Coda) → volver al segno → Tema de nuevo → Desarrollo → To Coda → saltar a sección Coda → terminar.
   - Preguntar: "Si no pongo el To Coda, ¿qué pasa en el D.S. al Coda?" (MuseScore no sabe a dónde saltar. El D.S. al Coda necesita que exista un To Coda Y una sección Coda. Si falta alguno, la navegación se rompe.)

5. **Barras de compás especiales** (5 min). Mostrar la paleta de Barras de compás:
   - **Simple**: la predeterminada.
   - **Doble**: cambio de sección. "Cuando cambia la armadura, el compás o el carácter de la música."
   - **Final**: barra fina + gruesa. "SOLO al final de la pieza o del movimiento."
   - **Punteada**: "Muy raramente usada. Divisiones no estándar."
   - **Momento de corrección**: "Muchos principiantes ponen barra final en cada cambio de sección. ESO ESTÁ MAL. La barra final le dice a MuseScore 'acá se terminó'. Si la ponés en el compás 16 de una pieza de 32 compases, MuseScore puede detener la reproducción ahí."
   - Demostrar: poner barra final en el compás 16. Reproducir: ¿se escucha lo que sigue? (Depende de la configuración, pero es una mala práctica.)

---

## 3. Práctica — Repeticiones, voltas y saltos de navegación

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S13 — Repeticiones, voltas y saltos de navegación

**Material**: el docente proporciona tres archivos:

1. **`ejercicio_S13_repeticiones.mscz`**: Partitura para piano (gran pentagrama) en Do mayor, 4/4, 32 compases con estructura A-B-A'.
   - **Sección A** (c.1–8): frase de 8 compases con carácter rítmico definido, melodía en mano derecha y acompañamiento simple en mano izquierda. Debe tener suficiente interés musical para que repetirla tenga sentido.
   - **Sección B** (c.9–16): frase contrastante (diferente registro, ritmo o carácter), también de 8 compases. La transición A→B debe ser natural pero perceptible.
   - **Sección A'** (c.17–32): reexposición variada de A. Los compases 17–24 forman el primer final (volta 1) y los compases 25–32 forman el segundo final (volta 2). El primer final debe terminar de manera "inconclusa" (ej. en dominante) para que la repetición tenga sentido. El segundo final debe tener un cierre más conclusivo.
   - El archivo se entrega SIN barras de repetición y SIN voltas. Todas las barras son simples.

2. **`ejercicio_S13_navegacion.mscz`**: Partitura para cuarteto de cuerdas (violín I, violín II, viola, violonchelo) en Sol mayor, 3/4, 28 compases.
   - **Introducción** (c.1–4): textura homofónica, tutti, carácter de apertura.
   - **Tema** (c.5–12): melodía en violín I, acompañamiento en los demás. Este tema debe "pedir" ser repetido después del desarrollo (por eso llevará el segno y el D.S. al Coda).
   - **Desarrollo** (c.13–24): variación del material del tema, textura más densa, modulaciones pasajeras.
   - **Coda** (c.25–28): 4 compases de cierre. Deben estar VACÍOS o con un esqueleto básico a completar por el docente. Llevan la etiqueta de texto "Coda".
   - El archivo se entrega SIN segno, SIN D.S., SIN To Coda, SIN Coda (solo las notas). Las barras de compás son todas simples.

3. **`ejercicio_S13_barras.mscz`**: Partitura para flauta sola en Fa mayor, 4/4, 16 compases.
   - Estructura A (c.1–4), B (c.5–8), C (c.9–12), Coda breve (c.13–16).
   - **Todas las barras de compás deben ser del tipo "simple"**, incluyendo la última. El texto "Sección B", "Sección C" aparece como Staff Text sobre los compases 5 y 9 para ayudar al estudiante a identificar los cambios.
   - La última nota (compás 16) es una redonda con calderón (opcional, para dar sensación de final).
   - El archivo debe tener al menos un lugar donde claramente se justifique una repetición (ej. la sección A es una frase que se repite casi idéntica en los compases 1–4, pero el estudiante debe detectarlo).

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Insertar barras de repetición en las secciones A y B del piano.
2. Insertar voltas 1 y 2 en la sección A' del piano.
3. Configurar D.S. al Coda completo en el cuarteto de cuerdas.
4. Corregir tipos de barras en la flauta (doble, final, repetición).
5. Diseñar una Coda propia y reconfigurar el mapa de navegación del piano.
6. Reflexionar sobre navegación musical.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Barras de repetición | Inicio y fin correctos en A y B; las 4 barras funcionales en reproducción | Repeticiones insertadas pero una sección no repite | Sin repeticiones o solo 1 sección |
| Voltas | Volta 1 y 2 correctamente colocadas; volta 1 termina en barra de repetición; secuencia 1ª/2ª vez correcta | Voltas insertadas pero mal extendidas o sin barra de repetición en volta 1 | Sin voltas o voltas no funcionales |
| D.S. al Coda | Segno, D.S. al Coda, To Coda y Coda colocados; navegación reproduce el orden correcto | Elementos presentes pero el orden de ejecución es incorrecto | Faltan elementos críticos o no funciona |
| Corrección de barras | Doble barra en ≥2 cambios de sección + barra final correcta; ≥4 cambios documentados | 2–3 cambios correctos o documentación incompleta | ≤1 cambio o sin documentación |
| Coda propia + navegación | 8 compases compuestos; segno reposicionado; D.S. al Coda funcional | Coda compuesta pero navegación falla en algún punto | Coda incompleta o navegación rota |
| Reflexión | 3 respuestas correctas con comprensión conceptual; ejemplos propios | 2 respuestas correctas | ≤1 respuesta correcta o superficial |

---

## 4. Cierre — El mapa de navegación

### Revisión por parejas (8 min)

Cada estudiante intercambia archivos con un compañero:
- Abre el archivo de piano del compañero. Reproduce la pieza completa: "¿Se repiten A y B correctamente? ¿Las voltas alternan bien? ¿La Coda propia tiene sentido en el mapa de navegación?"
- Abre el cuarteto de cuerdas del compañero. Sin mirar los saltos insertados, ESCUCHÁ la pieza y anotá el orden de las secciones: "¿La navegación es la correcta? ¿Falta algún elemento?"
- Abre la flauta del compañero: "¿Dónde pusiste las barras dobles? ¿Coinciden con mis decisiones?"

### Puesta en común (7 min)

Preguntas para guiar la discusión:
- "¿Qué fue más difícil: configurar las voltas o armar el D.S. al Coda?" (Esperado: el D.S. al Coda requiere coordinar 4 elementos distintos; si uno falla, todo se rompe. Es el verdadero desafío de la sesión.)
- "¿Por qué existen las voltas en lugar de simplemente escribir la música dos veces?" (Razones: ahorro de papel/tinta, menos trabajo de copia para el editor, el intérprete entiende la estructura musical más rápido. La repetición con voltas COMUNICA estructura.)
- "Si un D.S. al Coda no tiene To Coda, ¿qué pasa? ¿MuseScore muestra un error?" (MuseScore no muestra error explícito, simplemente no salta a la Coda. El estudiante tiene que diagnosticar por qué la navegación no funciona.)
- "¿En qué se diferencia un Fine de una barra final?" (Fine es una marca de navegación: indica dónde terminar DESPUÉS de un D.C. o D.S. La barra final es el fin absoluto de la pieza o movimiento. Pueden coexistir: Fine + barra final al final de todo.)
- "¿Alguna vez vieron una partitura que tuviera D.C. y D.S. en la misma pieza? ¿Tiene sentido?" (Puede tener sentido en formas complejas como rondós o arias da capo con variaciones internas. Pero en general, demasiados saltos confunden.)

### Resumen del docente (5 min)

1. Las repeticiones NO son un atajo para no escribir: son una herramienta de COMUNICACIÓN musical. Una barra de repetición le dice al intérprete "esta sección es importante, vale la pena escucharla dos veces". Una volta le dice "esta sección es igual excepto el final".
2. El D.S. al Coda es la estructura de navegación más compleja que van a usar en este curso. Si logran que funcione, entendieron el concepto. Los 4 elementos (segno, D.S., To Coda, Coda) son como piezas de un rompecabezas: si falta una, la imagen no se completa.
3. Las barras de compás tienen SIGNIFICADO. Una barra doble dice "cambio de sección". Una barra final dice "fin". Usarlas correctamente es parte de escribir partituras profesionales. La barra final en medio de la pieza es un error de principiante que grita "no revisé mi trabajo".
4. La reproducción de MuseScore es su mejor herramienta de verificación. Si la pieza no se reproduce en el orden esperado, ALGO está mal en el mapa de navegación. No asuman que está bien porque "se ve bien": escuchen.
5. Los mapas de navegación complejos (D.C., D.S., Coda) son comunes en música clásica, jazz, musicales y bandas sonoras. Saber leerlos y escribirlos correctamente es una habilidad profesional real.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| La repetición no funciona (no se repite) | Verificar que AMBAS barras (inicio y fin) estén insertadas. Si solo está la de fin, MuseScore asume repetición desde el principio, pero a veces no es suficiente si hay una barra de inicio explícita en otra parte. Insertar explícitamente la barra de inicio. |
| La volta 1 no se salta en la segunda pasada | Verificar que la volta 1 termine con barra de fin de repetición. Si termina con barra simple, MuseScore no entiende que hay que repetir y la volta no tiene efecto. |
| La volta 2 se toca en la primera pasada | Revisar la **lista de repetición** en Propiedades. Si la volta 2 tiene lista `1` en vez de `2`, se tocará en la primera pasada. Por defecto debería ser `2`, pero verificar si fue modificada accidentalmente. |
| El D.S. al Coda no salta a la Coda | Verificar que existan los 4 elementos: (1) segno en el lugar correcto, (2) D.S. al Coda en el lugar desde donde se salta, (3) To Coda en el lugar donde se abandona la sección, (4) marca Coda al inicio de la sección final. Si falta alguno, la navegación se rompe. |
| El segno no se ve o está mal posicionado | El segno debe arrastrarse sobre la BARRA de compás, no sobre una nota. Si se arrastró sobre una nota, puede quedar mal anclado. Borrar y volver a insertar sobre la barra. |
| El To Coda está en el lugar correcto pero la reproducción lo ignora | El problema puede ser que el D.S. al Coda no es "al Coda" sino "al Fine" (D.S. al Fine ignora el To Coda). Verificar que el salto sea específicamente D.S. al Coda. También verificar que el To Coda esté anclado a la barra y no a una nota. |
| El estudiante confunde marcas de ensayo (Ctrl+M) con segnos | Las marcas de ensayo son letras en un recuadro (A, B, C...) y NO afectan la reproducción. Los segnos (𝄋) son símbolos de navegación que SÍ afectan la reproducción. Son cosas completamente distintas. Si el estudiante pone una marca de ensayo esperando que haga de segno, no funcionará. |
| La barra final puesta en medio de la pieza detiene la reproducción | Si MuseScore tiene configurado "respetar barras finales", la reproducción se detiene al encontrar una. Solución: reemplazar por barra doble. Educar al estudiante: barra final = SOLO al final de todo. |
| El mapa de navegación de la Coda propia no funciona | Pedir al estudiante que dibuje el mapa EN PAPEL primero: un diagrama con flechas mostrando el orden de ejecución. Si no puede dibujarlo, probablemente no lo entendió. Luego implementarlo en MuseScore. |
| Demasiados saltos en una pieza corta, se vuelve confuso | Sugerir simplificar: ¿realmente necesita D.S. al Coda una pieza de 32 compases? A veces una simple barra de repetición con volta es más clara. Enseñar que la complejidad de navegación debe ser proporcional a la complejidad de la forma musical. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Repeats and jumps](https://handbook.musescore.org/notation/repeats-and-jumps.md)
- [MuseScore Studio Handbook — Voltas](https://handbook.musescore.org/notation/voltas.md)
- [MuseScore Studio Handbook — Barlines](https://handbook.musescore.org/notation/barlines.md)
- **Preparación del archivo `ejercicio_S13_repeticiones.mscz`**: crear partitura para piano en Do mayor, 4/4, 32 compases. Sección A (c.1–8): frase clara y memorable, melodía en mano derecha con ritmo definido (corcheas y negras), acompañamiento en mano izquierda con patrón rítmico simple. Sección B (c.9–16): frase contrastante (cambiar registro —subir una octava— o cambiar el patrón rítmico), también 8 compases. Sección A' (c.17–32): reexposición variada de A. Los compases 17–24 forman el primer final (terminar con cadencia a dominante, sensación de "inconcluso"). Los compases 25–32 forman el segundo final (cadencia conclusiva a tónica). Entregar con TODAS las barras como simples, SIN repeticiones y SIN voltas. La estructura A-B-A' debe ser musicalmente clara para que el estudiante sepa dónde poner las repeticiones.
- **Preparación del archivo `ejercicio_S13_navegacion.mscz`**: crear partitura para cuarteto de cuerdas en Sol mayor, 3/4, 28 compases. Introducción (c.1–4): textura homofónica, tutti, acordes en blancas. Tema (c.5–12): melodía en violín I, acompañamiento rítmico en los otros tres instrumentos. El tema debe ser lo suficientemente atractivo para que "merezca" ser repetido después del desarrollo. Desarrollo (c.13–24): variación y fragmentación del tema, modulaciones a tonalidades vecinas (Re mayor, Mi menor), textura más contrapuntística. Coda (c.25–28): 4 compases VACÍOS (el estudiante debe arrastrar la marca "Coda" desde la paleta de repeticiones). Entregar SIN segno, SIN D.S., SIN To Coda, SIN Coda (todo en barras simples).
- **Preparación del archivo `ejercicio_S13_barras.mscz`**: crear partitura para flauta sola en Fa mayor, 4/4, 16 compases. Sección A (c.1–4): frase lírica. Sección B (c.5–8): frase más rítmica. Sección C (c.9–12): frase contrastante en registro. Coda (c.13–16): cierre con calderón en la última nota. Colocar Staff Text "Sección B" sobre el compás 5 y "Sección C" sobre el compás 9. Entregar con TODAS las barras como simples (incluso la última). Opcional: hacer que la sección A (c.1–4) sea casi idéntica a como empieza la sección B (c.5–8), de modo que un estudiante atento pueda sugerir que la sección A debería repetirse.
- Dato curioso: los signos de repetición con barras y puntos (como los conocemos hoy) se estandarizaron en el siglo XVII. Antes de eso, las repeticiones se escribían con palabras como "bis" o se sobreentendían por la forma musical. Los símbolos de D.C., D.S. y Coda provienen del italiano (el idioma estándar de la notación musical desde el Renacimiento) y se han mantenido sin cambios durante siglos.
- Dato curioso: en la era de la copia manual de partituras (antes de la imprenta musical), las repeticiones NO eran una conveniencia: eran una NECESIDAD. Copiar una pieza entera a mano llevaba horas. Cada sección que se repetía sin tener que reescribirla ahorraba tiempo, tinta y pergamino. Las voltas y los saltos de navegación son, en cierto sentido, una de las primeras "optimizaciones de espacio" de la historia de la información.
- Ejercicio opcional de ampliación: entregar a los estudiantes una partitura real de una sonata clásica (Haydn o Mozart, primer movimiento) y pedirles que identifiquen todas las barras de repetición, voltas y saltos de navegación. Luego, dibujar el "mapa de navegación" de la sonata en papel. Es un excelente ejercicio de análisis formal que conecta la notación con la forma musical.

---

*Guía docente — Tecnología Musical I | Sesión 13*
