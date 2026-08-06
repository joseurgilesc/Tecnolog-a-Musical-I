# Sesión 23: Importación y limpieza de archivos MIDI

📚 Handbook → Advanced topics: MIDI import | Herramientas: MuseScore Studio 4, Google Classroom, archivos MIDI de referencia

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="importacion-midi"></a> **Importación MIDI** | Proceso de abrir un archivo MIDI (.mid, .midi, .kar) en MuseScore y convertirlo automáticamente en una partitura con notas, pentagramas, claves e indicaciones de compás. MuseScore "traduce" el archivo MIDI (instrucciones) a notación musical (pentagrama). La calidad del resultado depende de la calidad del archivo MIDI original. |
    | <a id="cuantizacion-import"></a> **Cuantización en importación** | Parámetro que controla cómo MuseScore simplifica los ritmos del MIDI durante la importación. Valores más altos (negra, blanca) simplifican más (ignoran subdivisiones rápidas). Valores más bajos (fusa, semifusa) preservan los detalles rítmicos pero pueden generar notación excesivamente compleja y difícil de leer. |
    | <a id="midi-type"></a> **Tipos de archivo MIDI (Type 0 vs Type 1)** | Type 0: todas las pistas MIDI combinadas en UNA sola pista (monolítico). Type 1: múltiples pistas separadas (multipista). MuseScore maneja ambos tipos, pero los archivos Type 1 producen mejores resultados porque cada pista puede mapearse a un pentagrama independiente. Los archivos .KAR (karaoke) son Type 0 con letra embebida. |
    | <a id="canal-midi-import"></a> **Canal MIDI en importación** | Cada pista de un archivo MIDI está asignada a un canal (1–16). Durante la importación, MuseScore intenta detectar qué canal corresponde a qué instrumento (canal 10 = percusión por convención, canales 1–9 y 11–16 = instrumentos melódicos). Si el archivo MIDI tiene una asignación extraña, los instrumentos pueden quedar mal mapeados. |
    | <a id="mapeo-instrumentos"></a> **Mapeo de instrumentos MIDI** | Proceso de convertir los mensajes "Program Change" del archivo MIDI (que indican "sonido de piano", "sonido de violín", etc.) en instrumentos de MuseScore. El estándar General MIDI (GM) define 128 sonidos numerados: 1 = Acoustic Grand Piano, 41 = Violin, 57 = Trumpet. Si el archivo MIDI sigue el estándar GM, la importación asigna los instrumentos automáticamente. |
    | <a id="overlapping-notes"></a> **Notas superpuestas (overlapping notes)** | Problema común en archivos MIDI importados donde dos notas del MISMO instrumento y misma altura se solapan en el tiempo (una empieza antes de que la anterior termine). MuseScore las interpreta como voces separadas o como ligaduras incorrectas. Pueden generar pentagramas con aspecto "sucio" y difícil de leer. |
    | <a id="pedal-midi"></a> **Pedal de sustain (CC64) en MIDI** | Mensaje MIDI que indica cuándo se pisa y se suelta el pedal de sustain del piano. En la importación, MuseScore puede ignorarlo, representarlo como líneas de pedal en la partitura, o interpretarlo como notas prolongadas (ligaduras). El comportamiento depende de la configuración de importación. |
    | <a id="microdesplazamiento"></a> **Microdesplazamiento rítmico** | Pequeñas imprecisiones temporales en un archivo MIDI (porque el intérprete original tocó "adelantado" o "atrasado" respecto al metrónomo). Durante la importación, estos microdesplazamientos pueden generar figuras rítmicas extrañas: una corchea "casi a tiempo" puede importarse como una nota con puntillo, una semicorchea con silencio previo, o valores irregulares. |
    | <a id="limpieza-midi"></a> **Limpieza de partitura MIDI** | Proceso posterior a la importación que incluye: eliminar pentagramas innecesarios, fusionar voces duplicadas, corregir alteraciones enarmónicas (Do♯ convertido en Re♭ sin razón), normalizar las direcciones de plica, eliminar silencios excesivos, ajustar la cuantización y verificar la asignación de instrumentos. Es la parte que consume más tiempo en el flujo MIDI → partitura. |
    | <a id="general-midi"></a> **General MIDI (GM)** | Estándar de la industria que define un conjunto de 128 sonidos numerados (piano, guitarra, cuerdas, etc.) y su asignación a canales (canal 10 = percusión). Adoptado en 1991, GM garantiza que un archivo MIDI suene "parecido" en cualquier dispositivo compatible. MuseScore usa GM como referencia para el mapeo de instrumentos durante la importación. |
    | <a id="midi-karaoke"></a> **MIDI Karaoke (.KAR)** | Formato de archivo MIDI que incluye letras de canciones incrustadas como metadatos (eventos de texto y letra). MuseScore puede importar archivos .KAR y extraer automáticamente la letra como Lyrics en el pentagrama correspondiente. Es el formato típico de archivos MIDI "con pista de voz" que se usan en karaoke. |
    | <a id="program-change"></a> **Program Change** | Mensaje MIDI que ordena a un dispositivo cambiar el sonido que está usando. "Program 1" = Acoustic Grand Piano, "Program 41" = Violin. En un archivo MIDI, cada pista tiene un Program Change al inicio que indica qué instrumento debe sonar. Durante la importación, MuseScore usa estos mensajes para asignar instrumentos a los pentagramas. |

???+ note "¿Para qué importar archivos MIDI?"

    La importación MIDI es uno de los flujos de trabajo más potentes de MuseScore, pero también uno de los más incomprendidos. No es "magia negra que convierte cualquier cosa en partitura". Es una HERRAMIENTA que funciona bien con ciertos tipos de archivos y mal con otros.

    ### Cuándo SÍ importar MIDI

    | Situación | ¿Por qué funciona? |
    |---|---|
    | **Archivo MIDI exportado desde otro editor de partituras** (Finale, Sibelius, Dorico, el mismo MuseScore) | El MIDI fue GENERADO desde una partitura. La cuantización es perfecta. Los ritmos son exactos. La importación es casi perfecta. |
    | **Archivo MIDI de un secuenciador por pasos** (patrones de batería, líneas de bajo programadas en un DAW) | Las notas fueron "dibujadas" en una grilla, no tocadas. Alta precisión rítmica. |
    | **Archivo MIDI de una interpretación cuantizada** (el pianista tocó y luego aplicó cuantización en el DAW) | Si la cuantización es fuerte (> 80%), los ritmos son aceptables. Algo de limpieza necesaria. |
    | **Archivo .KAR de karaoke** | Suele tener melodía bien definida y letra incrustada. La importación extrae ambos. |
    | **MIDI Type 1 multipista** (cada instrumento en su propia pista) | MuseScore puede separar las pistas en pentagramas independientes automáticamente. |

    ### Cuándo NO importar MIDI

    | Situación | ¿Por qué NO funciona bien? |
    |---|---|
    | **Grabación en vivo sin cuantizar** (un pianista tocando libremente) | Lleno de microdesplazamientos, notas superpuestas, pedales interpretados como notas largas. El resultado será una partitura ILEGIBLE. |
    | **Archivo MIDI de una orquesta completa en Type 0** | Todas las pistas combinadas en una sola. MuseScore no puede separar instrumentos. Aparecerán decenas de pentagramas con nombres genéricos "Pista 1", "Pista 2". |
    | **Improvisación libre de jazz** | Ritmos irregulares, swing, rubato. La notación resultante será una pesadilla de tresillos, quintillos y valores irregulares. |
    | **Música microtonal o con bending** | MIDI permite pitch bend, pero la notación estándar NO. Las notas "desafinadas" del MIDI se redondean al semitono más cercano. |
    | **Archivo MIDI corrupto o mal formado** | Notas faltantes, duraciones negativas, canales mal asignados. La importación falla parcial o totalmente. |

    !!! tip "Regla de oro de la importación MIDI"
        **Cuanto más "mecánico" y "programado" sea el archivo MIDI, mejor será la importación. Cuanto más "humano" y "expresivo", peor.** El MIDI generado desde una partitura se importa casi perfecto. El MIDI grabado desde un teclado en vivo requiere trabajo de limpieza. Aceptá esta realidad y planificá tu tiempo en consecuencia.

    ### El flujo de trabajo típico

    1. **Importar** el MIDI con parámetros conservadores.
    2. **Evaluar** el resultado: ¿es usable? ¿O es un desastre?
    3. Si es un desastre → OPCIONES: (a) buscar otra fuente MIDI, (b) cuantizar el archivo original en un DAW y reimportar, (c) transcribir manualmente desde cero (a veces es más rápido).
    4. Si es usable → **Limpiar**: pentagramas, enarmonías, plicas, silencios, voicing.
    5. **Verificar**: ¿lo que está escrito suena como el MIDI original?

???+ note "Importación paso a paso"

    ### Abrir un archivo MIDI en MuseScore

    1. **Archivo → Abrir** (o `Ctrl / Cmd + O`).
    2. Navegar hasta el archivo MIDI (.mid, .midi, .kar).
    3. Seleccionarlo y hacer clic en **Abrir**.

    MuseScore NO abre el MIDI directamente. En su lugar, muestra un **diálogo de importación** con opciones que afectan drásticamente el resultado.

    ### Parámetros del diálogo de importación

    | Parámetro | Qué hace | Recomendación |
    |---|---|---|
    | **Cuantización más corta** | Define la figura rítmica más pequeña que MuseScore intentará detectar. "Semicorchea" es buena para la mayoría de casos. "Fusa" captura más detalle pero produce partituras sobrecargadas. | Empezar con **semicorchea**. Si la partitura resultante es demasiado simple (faltan notas rápidas), bajar a fusa. Si es demasiado compleja, subir a corchea. |
    | **Número máximo de voces por pentagrama** | Define cuántas voces independientes detectará MuseScore. Para piano: 2 voces (melodía + acompañamiento en una misma mano). Para música orquestal: 1 voz por pentagrama. | Piano: 2 voces. Ensamble: 1–2 voces. Si hay notas superpuestas, aumentar. |
    | **Simplificar duraciones** | Fusiona silencios pequeños y notas ligadas para limpiar la notación. Activado = partitura más legible pero menos fiel al original. | **Activado** generalmente. Desactivar solo si necesitás precisión absoluta (ej. transcripción musicológica). |
    | **Mostrar líneas de pedal** | Convierte los mensajes CC64 (pedal de sustain) en líneas de pedal visibles en la partitura. | **Activado** para música de piano. Desactivado para otros instrumentos. |
    | **Usar alteraciones enarmónicas** | Convierte Do♯ en Re♭ automáticamente según la armadura. | **Activado**. Reduce el trabajo de limpieza posterior. |

    ### Después de la importación: el diagnóstico

    Apenas se abre el MIDI, hacé estas 3 verificaciones:

    1. **¿Los instrumentos son correctos?** Verificá que cada pentagrama tenga asignado el instrumento adecuado. Si el MIDI tenía "Piano" pero MuseScore lo abrió como "Violín", cambiá el instrumento en **Propiedades del pentagrama**.
    2. **¿La armadura y el compás son correctos?** MuseScore intenta detectarlos, pero puede fallar. Verificá al inicio de la partitura.
    3. **¿Hay pentagramas duplicados o innecesarios?** Archivos Type 1 con muchas pistas MIDI generan muchos pentagramas. "Pista 3", "Pista 7" son nombres genéricos. Eliminá los que no uses.


???+ note "Limpieza de partitura importada: los 7 problemas clásicos"

    La importación MIDI casi nunca es perfecta. Estos son los 7 problemas más frecuentes y cómo resolverlos. Aprendelos: te ahorrarán horas de frustración.

    ### Problema 1: Ritmos extraños (tresillos falsos, puntillos innecesarios)

    **Causa**: el intérprete original tocó con pequeñas imprecisiones rítmicas.

    **Solución**:
    - Seleccionar el pasaje problemático.
    - **Herramientas → Cuantizar...** o **Editar → Cuantización** (en algunas versiones: **Formato → Cuantizar**).
    - Elegir la figura de cuantización (negra, corchea, semicorchea).
    - Aplicar y verificar: ¿los ritmos ahora tienen sentido musical?

    **Ejemplo**: un pasaje que debería ser "corchea-corchea-negra" pero el MIDI lo muestra como "corchea con puntillo-semicorchea-negra con puntillo" → cuantizar a corchea lo corrige.

    ### Problema 2: Notas superpuestas y ligaduras falsas

    **Causa**: el intérprete no soltó una nota antes de tocar la siguiente (legato exagerado, pedal sostenido).

    **Solución**:
    - Identificar las notas superpuestas: se ven como dos notas iguales que empiezan en tiempos ligeramente distintos y se ligan entre sí.
    - Seleccionar la nota que sobra y eliminarla (`Supr`).
    - Si hay muchas: **Editar → Seleccionar → Más...** → seleccionar "Nota" con duración mínima (ej. todas las notas más cortas que una semicorchea) → eliminar.

    ### Problema 3: Armadura incorrecta o ausente

    **Causa**: el archivo MIDI no contiene información de armadura. MuseScore asume Do mayor / La menor por defecto.

    **Solución**:
    - Escuchar la partitura. Identificar la tonalidad de oído.
    - Arrastrar la armadura correcta desde la paleta **Armaduras** al primer compás.
    - MuseScore ajustará automáticamente las alteraciones accidentales (convierte sostenidos/bemoles según la nueva armadura).
    - Verificar compás por compás que las alteraciones sean correctas.

    ### Problema 4: Enarmonías incorrectas (Do♯ en lugar de Re♭)

    **Causa**: el MIDI solo transmite el número de nota (altura en semitonos sobre Do₀). No distingue entre Do♯ y Re♭ porque son la MISMA altura MIDI. MuseScore tiene que "adivinar" cuál escribir.

    **Solución**:
    - Seleccionar la nota con la enarmonía incorrecta.
    - Presionar `J` (cambia entre las representaciones enarmónicas disponibles).
    - O hacer clic derecho → **Propiedades de la nota → Alteración → elegir la correcta**.
    - Regla general: en tonalidades con sostenidos, preferir Do♯ sobre Re♭. En tonalidades con bemoles, preferir Re♭ sobre Do♯. La nota DEBE ser fácil de leer en el contexto de la armadura.

    ### Problema 5: Pentagramas con nombres genéricos y instrumentos mal asignados

    **Causa**: el archivo MIDI usa nombres de pista no estándar o carece de mensajes Program Change.

    **Solución**:
    - Clic derecho en el nombre del pentagrama → **Propiedades del pentagrama**.
    - **Cambiar instrumento** → buscar el instrumento correcto.
    - Renombrar la pista con un nombre descriptivo ("Violín I" en lugar de "Pista 3").
    - Si hay instrumentos que no aparecen en la partitura (percusión que se asignó a un pentagrama melódico), verificar el canal MIDI: canal 10 debe ser percusión.

    ### Problema 6: Plicas inconsistentes y dirección errónea

    **Causa**: MuseScore asigna dirección de plica automáticamente, pero en música importada las decisiones automáticas pueden ser incorrectas.

    **Solución**:
    - Seleccionar las notas afectadas.
    - **Propiedades → Plica → Dirección**: elegir "Arriba", "Abajo" o "Automático" según corresponda.
    - Para pasajes con voces mezcladas, verificar que la voz 1 (plica arriba) y voz 2 (plica abajo) sean consistentes.

    ### Problema 7: Dinámicas y cambios de tempo pegados a notas incorrectas

    **Causa**: los mensajes CC (control change) de volumen y los mensajes de tempo del MIDI se convierten en marcas de dinámica y tempo de MuseScore, pero pueden quedar "anclados" a notas incorrectas.

    **Solución**:
    - Reproducir la partitura. Si una dinámica o cambio de tempo ocurre en un momento extraño, seleccionarlo, eliminarlo y reinsertarlo manualmente.
    - Las dinámicas MIDI (CC7 = volumen) suelen ser problemáticas porque representan el volumen ABSOLUTO del canal, no una indicación musical. Generalmente es mejor eliminarlas todas y reescribir las dinámicas manualmente.


???+ note "Importación avanzada: configuraciones especiales"

    ### Importar batería y percusión desde MIDI

    Los archivos MIDI de batería pueden importarse correctamente SI el archivo sigue el estándar General MIDI para percusión (canal 10 con el mapa estándar de notas de percusión):

    1. Importar el archivo normalmente (o arrastrarlo a MuseScore).
    2. En el diálogo de importación, asegurarse de que el canal 10 esté asignado al pentagrama de Drumset.
    3. Si MuseScore no detecta la percusión automáticamente: después de la importación, clic derecho en el pentagrama → **Cambiar instrumento → Percusión no afinada → Drumset**.
    4. Las cabezas de nota deberían cambiar automáticamente (X para platillos, circular para tambores). Si no lo hacen, verificar el mapa de percusión del pentagrama.

    ### Importar MIDI con pista de letra (karaoke .KAR)

    1. Abrir el archivo .KAR con **Archivo → Abrir**.
    2. MuseScore detecta la pista de letra y la coloca como **Lyrics** debajo del pentagrama correspondiente.
    3. Verificar la sincronización: la letra debe estar alineada con las notas correctas. Si no lo está, ajustar manualmente moviendo las sílabas con `Ctrl + → / ←`.
    4. La letra importada puede contener caracteres no deseados (códigos de sincronización, marcas de karaoke como "/" para separación de sílabas). Limpiarlos manualmente.

    ### Importación por arrastre (drag and drop)

    Alternativa rápida: arrastrar el archivo MIDI directamente desde el Explorador de archivos (Windows) o Finder (Mac) a la ventana de MuseScore. El diálogo de importación aparece igual y el proceso es idéntico.

---

## Actividad en Classroom

### Tarea: S23 — Importación y limpieza de archivos MIDI

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S23_melodia.mid`, un archivo MIDI Type 1 de una melodía para flauta y acompañamiento de piano, bien cuantizado y con asignación correcta de instrumentos, listo para importar con pocos problemas; (b) `ejercicio_S23_desastre.mid`, un archivo MIDI Type 1 deliberadamente "problemático" con microdesplazamientos, enarmonías incorrectas, 3 pentagramas con nombres genéricos, y notas superpuestas, simulando una grabación en vivo sin cuantizar; (c) `ejercicio_S23_karaoke.kar`, un archivo .KAR con una canción popular en español que incluya melodía, acompañamiento y letra.

1. **Importación limpia: diagnóstico.** Abrí `ejercicio_S23_melodia.mid` en MuseScore con los parámetros recomendados (cuantización: semicorchea, voces: 1 por pentagrama, simplificar duraciones: activado, líneas de pedal: activado, enarmonías: activado):
    - Describí el resultado: ¿cuántos pentagramas se generaron? ¿Los instrumentos son correctos? ¿La armadura y el compás coinciden con lo que escuchás?
    - Verificá que la melodía de flauta y el acompañamiento de piano estén en pentagramas separados y correctamente nombrados.
    - Reproducí la partitura. ¿Suena igual que el MIDI original? Si no, ¿dónde están las diferencias?
    - Este es el "caso ideal": un MIDI bien hecho. Documentá qué parámetros de importación usaste y si hubo que hacer algún ajuste.

2. **Limpieza de archivo problemático.** Abrí `ejercicio_S23_desastre.mid` en MuseScore:
    - **Diagnóstico**: observá la partitura resultante. Identificá al menos CINCO problemas de los 7 tipos estudiados (ritmos extraños, notas superpuestas, armadura incorrecta, enarmonías, pentagramas genéricos, plicas inconsistentes, dinámicas mal ubicadas). Anotalos.
    - **Cuantización**: seleccioná toda la partitura y aplicá cuantización a corchea. ¿Mejoró? Probá con semicorchea. ¿Cuál da mejor resultado? Documentá.
    - **Pentagramas**: renombrá los pentagramas con nombres de instrumentos reales. Asigná el instrumento correcto si MuseScore no lo detectó. Eliminá pentagramas innecesarios.
    - **Enarmonías**: corregí al menos 10 notas con enarmonías incorrectas usando `J` o las propiedades de la nota.
    - **Notas superpuestas**: encontrá al menos 5 pares de notas superpuestas y eliminalas.
    - **Plicas**: normalizá la dirección de plicas en al menos 2 pasajes donde sean inconsistentes.
    - **Dinámicas**: eliminá las marcas de dinámica automáticas que quedaron mal ubicadas. Agregá manualmente al menos 4 marcas de dinámica (`p`, `mf`, `f`, `ff`) y un regulador (crescendo/diminuendo).
    - **Resultado final**: exportá la partitura limpia como PDF y MSCZ. La partitura debe ser legible, con los instrumentos correctos, ritmos musicalmente coherentes y una presentación profesional.

3. **Karaoke MIDI: letra y melodía.** Abrí `ejercicio_S23_karaoke.kar` en MuseScore:
    - Verificá que la letra se haya importado como **Lyrics** debajo de las notas correctas.
    - Si hay errores de sincronización (letra en notas incorrectas), corregilos moviendo las sílabas con `Ctrl + → / ←` o reescribiendo la letra manualmente.
    - Limpiá caracteres extraños típicos de archivos .KAR (códigos de sincronización, barras "/", guiones dobles).
    - Identificá la melodía principal y las pistas de acompañamiento. Nombrá cada pentagrama correctamente.
    - Agregá el cifrado armónico (`Ctrl + K`) sobre la melodía si la canción tiene una progresión de acordes reconocible (escuchá el acompañamiento).
    - Exportá como PDF.

4. **Integración: partitura desde MIDI.** Buscá en internet o en tu biblioteca personal UN archivo MIDI de tu elección que cumpla con estos requisitos:
    - Debe ser Type 1 (multipista), NO Type 0.
    - Debe tener al menos 4 instrumentos diferentes (ej. piano, bajo, batería, melodía).
    - Debe ser música que reconozcas y te guste (para que puedas evaluar si la importación "suena bien").
    - No uses archivos de karaoke (.KAR) para este ejercicio.

    Creá una carpeta y guardá el archivo como `APELLIDO_Nombre_S23_midi_original.mid`. Luego:
    - **Importá** el MIDI en MuseScore con los parámetros que consideres adecuados. Documentá qué parámetros usaste y por qué.
    - **Limpiá** la partitura siguiendo el flujo de los 7 problemas. Documentá en un comentario de Classroom los problemas que encontraste y cómo los resolviste.
    - **Mejorá** la partitura: agregá nombre de compositor, título de la obra, indicaciones de tempo, dinámicas razonables, y cualquier marca de expresión que consideres necesaria.
    - Guardá como `APELLIDO_Nombre_S23_midi_importado.mscz`.
    - Exportá como PDF y como audio (MP3 o WAV) para comparar con el MIDI original.

5. **Reflexión sobre importación MIDI.** En Classroom, respondé:
    - ¿Qué tipo de archivos MIDI se importan mejor y por qué? Describí las características del archivo que produjo la mejor importación en tu experiencia (propia o de los ejercicios).
    - ¿Cuál de los 7 problemas de limpieza te resultó más difícil de resolver? ¿Qué estrategia usaste para resolverlo?
    - Compará el tiempo que te llevó limpiar `ejercicio_S23_desastre.mid` con el tiempo estimado que te habría llevado escribir esa misma partitura desde cero. ¿Cuándo conviene importar y limpiar vs. empezar desde cero?

### Entregables

- [ ] `APELLIDO_Nombre_S23_melodia_v01.mscz` (importación limpia, pocos ajustes)
- [ ] `APELLIDO_Nombre_S23_melodia_v01.pdf`
- [ ] `APELLIDO_Nombre_S23_desastre_v01.mscz` (archivo problemático completamente limpiado)
- [ ] `APELLIDO_Nombre_S23_desastre_v01.pdf`
- [ ] `APELLIDO_Nombre_S23_karaoke_v01.mscz` (karaoke con letra corregida y cifrado)
- [ ] `APELLIDO_Nombre_S23_karaoke_v01.pdf`
- [ ] `APELLIDO_Nombre_S23_midi_original.mid` (el archivo MIDI que elegiste)
- [ ] `APELLIDO_Nombre_S23_midi_importado_v01.mscz` (tu partitura importada y mejorada)
- [ ] `APELLIDO_Nombre_S23_midi_importado_v01.pdf`
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) lista de los 5+ problemas identificados en `ejercicio_S23_desastre.mid` y cómo los resolviste, (c) enlace o nombre del archivo MIDI que elegiste en la Parte 4 y por qué lo elegiste

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Importación limpia | Parámetros correctos; instrumentos y armadura verificados; sin errores de importación | Importación correcta pero sin verificación de instrumentos o armadura | Importación no realizada o con parámetros incorrectos |
| Limpieza de archivo problemático | ≥5 problemas identificados y resueltos; cuantización probada; enarmonías corregidas; pentagramas renombrados; resultado legible y profesional | 3–4 problemas resueltos o limpieza incompleta | ≤2 problemas resueltos |
| Karaoke MIDI | Letra importada y sincronizada; caracteres extraños limpiados; pentagramas nombrados; cifrado armónico agregado | Letra importada pero con errores de sincronización o sin limpiar | Karaoke no procesado |
| Integración (MIDI propio) | Archivo Type 1 con ≥4 instrumentos; importación documentada; limpieza completa; partitura mejorada con metadatos y dinámicas | Archivo importado pero con limpieza parcial o <4 instrumentos | Archivo no importado o tipo incorrecto |
| Reflexión | 3 respuestas con análisis técnico; comparación importar vs. escribir desde cero; mención de tipos de archivo y problemas | 2 respuestas correctas | ≤1 respuesta o superficial |

---

*Basado en: MuseScore Studio 4 Handbook — MIDI import | https://handbook.musescore.org*
