# Guía Docente — Sesión 23: Importación y limpieza de archivos MIDI

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivos `ejercicio_S23_melodia.mid`, `ejercicio_S23_desastre.mid` y `ejercicio_S23_karaoke.kar` preparados por el docente  
**Referencia:** MuseScore Studio Handbook — MIDI import

---

## Objetivo de la sesión

Que el estudiante domine el diálogo de importación MIDI comprendiendo el efecto de cada parámetro en el resultado final, diagnostique y resuelva los 7 problemas clásicos de las partituras importadas (ritmos extraños, notas superpuestas, enarmonías incorrectas, pentagramas genéricos, plicas inconsistentes, armaduras erróneas y dinámicas mal ubicadas), y desarrolle criterio para decidir cuándo conviene importar y limpiar un archivo MIDI versus cuándo es más eficiente escribir la partitura desde cero.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S22 + pregunta disparadora: ¿importar MIDI es magia o herramienta? |
| **Desarrollo** | 35 min | Demostración: importación limpia → archivo problemático y los 7 problemas → karaoke |
| **Práctica** | 60 min | Importación limpia → limpieza del desastre → karaoke → integración con MIDI propio |
| **Cierre** | 15 min | Comparación de estrategias, puesta en común, entrega |

---

## 1. Apertura — ¿Magia o herramienta?

### Materiales
- Proyector con MuseScore Studio abierto.
- Los archivos `ejercicio_S23_melodia.mid`, `ejercicio_S23_desastre.mid` y `ejercicio_S23_karaoke.kar` publicados en Classroom **antes de la clase**.
- Parlantes funcionales para reproducir los MIDI.

### Dinámica

1. **Revisión de S22** (5 min):
   - ¿Alguien logró conectar su teclado MIDI esta semana? ¿Step-time o real-time?
   - Rápidamente: ¿MIDI es audio? (No.) ¿Qué es? (Instrucciones.) Bien, hoy usamos archivos MIDI, no teclados.

2. **Preguntas disparadoras** (5 min):
   - Proyectar una partitura de 4 páginas completamente escrita. "¿Cuánto tiempo creen que me llevó escribir esto?" (Esperar respuestas: 2 horas, 3 horas.)
   - "La escribí en 30 segundos. La importé desde un archivo MIDI." (Pausa para efecto.)
   - "Ahora... ¿está bien escrita? Miremos más de cerca." (Hacer zoom en pasajes con errores típicos deliberados: ritmos raros, enarmonías mal, notas superpuestas.)
   - "La importación MIDI es el equivalente a un borrador generado por IA: te ahorra el 80% del trabajo, pero el 20% que queda ES TU RESPONSABILIDAD. Si no lo limpiás, tu partitura es un desastre. Si lo limpiás bien, nadie sabrá que no la escribiste nota por nota."
   - "¿Alguna vez descargaron un MIDI de internet y lo abrieron en MuseScore? ¿Se veía bien o era un desastre?" (La mayoría dirá que era un desastre. Validar la experiencia y anticipar que hoy aprenderán a DOMINAR ese desastre.)

---

## 2. Desarrollo — Del caos a la partitura

### Secuencia sugerida

1. **Importación limpia: el caso ideal** (8 min). Con `ejercicio_S23_melodia.mid`:
   - "Este archivo MIDI fue exportado desde otro editor de partituras. Vean qué pasa."
   - Abrir **Archivo → Abrir** → seleccionar el MIDI.
   - Mostrar el diálogo de importación. Explicar CADA opción:
     - **Cuantización más corta**: "Define la figura más pequeña que MuseScore 'escucha'. Semicorchea = atrapa semicorcheas y todo lo más lento. Fusa = captura notas muy rápidas pero genera más ruido."
     - **Número máximo de voces**: "Para piano pueden ser 2 (melodía + acompañamiento en una mano). Para orquesta, 1. Si hay muchas notas superpuestas, subir a 3."
     - **Simplificar duraciones**: "Limpia silencios y ligaduras innecesarias. Activado para la mayoría de casos."
     - **Líneas de pedal**: "Para piano SÍ. Para flauta NO."
     - **Enarmonías**: "Activado = Do♯ se convierte en Re♭ si la armadura lo pide."
   - "Vean el resultado: flauta en un pentagrama, piano en su gran pentagrama. Armadura correcta. Compás 4/4. Ritmos limpios."
   - **Lección**: "Cuando el MIDI viene de una PARTITURA, la importación es casi automática. El problema es cuando el MIDI viene de una GRABACIÓN."

2. **Los 7 problemas clásicos** (18 min). Con `ejercicio_S23_desastre.mid`:
   - Importar con parámetros por defecto y mostrar el resultado en pantalla. Se va a ver HORRIBLE. Ritmos extraños por todos lados.
   - "Este archivo simula lo que pasa cuando importás una grabación en vivo SIN cuantizar. Vean el caos."
   - Recorrer los 7 problemas uno por uno, en vivo, mostrando el "antes" horrible y el "después" limpio:

     **(1) Ritmos extraños** (3 min):
     - Seleccionar 4 compases llenos de tresillos falsos y puntillos extraños.
     - **Herramientas → Cuantizar → corchea**. ¡Puf! La mayoría de los ritmos se normalizan.
     - "La cuantización es como un filtro que redondea los ritmos a la figura más cercana. Probá con corchea primero. Si falta detalle, bajá a semicorchea."

     **(2) Notas superpuestas** (3 min):
     - Señalar notas que se solapan (misma altura, empiezan en tiempos ligeramente distintos).
     - "Esto pasa cuando el pianista no soltó el pedal a tiempo. Son 'fantasmas'."
     - Mostrar cómo eliminarlas manualmente y con selección masiva.

     **(3) Armadura incorrecta** (2 min):
     - "El MIDI no trae armadura. MuseScore asume Do mayor."
     - Escuchar la pieza. Identificar que está en Re mayor. Arrastrar la armadura de 2 sostenidos.
     - "Vean cómo todas las alteraciones accidentales DESAPARECEN. MuseScore ajustó todo automáticamente."

     **(4) Enarmonías** (2 min):
     - Señalar un Sol♯ que debería ser La♭. "Misma tecla en el piano, diferente significado musical."
     - Seleccionar → `J`. "Un atajo. Una tecla. Resuelto."
     - "Regla: si la tonalidad tiene sostenidos, usá sostenidos. Si tiene bemoles, usá bemoles."

     **(5) Pentagramas genéricos** (2 min):
     - "Pista 1", "Pista 3", "Pista 7"... "¿Esto es una orquesta o un estacionamiento?"
     - Clic derecho → Propiedades del pentagrama → Cambiar instrumento.
     - Eliminar pentagramas duplicados o vacíos con **Editar → Instrumentos**.

     **(6) Plicas inconsistentes** (3 min):
     - Mostrar un pasaje donde algunas plicas van para arriba y otras para abajo sin sentido musical.
     - Seleccionar todo → Propiedades → Plica → Dirección → Automático.
     - "MuseScore vuelve a calcular la dirección según las reglas de notación estándar."

     **(7) Dinámicas fantasma** (3 min):
     - "Los mensajes CC del MIDI se convierten en dinámicas que quedan pegadas a notas aleatorias."
     - Seleccionar todas las marcas de dinámica incorrectas → `Supr`.
     - "Generalmente es mejor BORRAR todas las dinámicas automáticas y reescribirlas manualmente. Las que importa MuseScore desde MIDI casi nunca son musicalmente correctas."

   - Mostrar el resultado final: "Miren el antes y el después. De un desastre ilegible a una partitura profesional. En 15 minutos de limpieza."

3. **Karaoke MIDI** (5 min). Con `ejercicio_S23_karaoke.kar`:
   - "Los archivos .KAR son MIDI con letra. MuseScore los importa y extrae la letra automáticamente."
   - Abrir el archivo. Mostrar cómo la letra aparece debajo de las notas del pentagrama melódico.
   - Señalar problemas típicos: sincronización (letra corrida respecto a las notas), caracteres extraños ("/", "_", códigos de karaoke).
   - Corregir en vivo: mover sílabas con `Ctrl + →`, borrar caracteres extraños.
   - "Si alguna vez necesitaron la letra de una canción sincronizada con la partitura, el formato .KAR es su mejor amigo."

4. **Decisión crítica: ¿importar o escribir?** (4 min). 
   - "Después de esta demostración, la pregunta obvia es: ¿vale la pena? ¿No es más rápido escribir todo desde cero?"
   - Poner en el pizarrón:
     - MIDI de partitura → importar (5% de limpieza) >>> escribir desde cero.
     - MIDI de grabación cuantizada → importar (30% de limpieza) ≈ escribir desde cero (depende de la complejidad).
     - MIDI de grabación SIN cuantizar → escribir desde cero ES MÁS RÁPIDO.
   - "No hay una respuesta universal. Hay criterio. Y el criterio se desarrolla con experiencia. Hoy están adquiriendo esa experiencia."

---

## 3. Práctica — El laboratorio de limpieza MIDI

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S23 — Importación y limpieza de archivos MIDI

**Material**: el docente proporciona tres archivos:

1. **`ejercicio_S23_melodia.mid`**: Archivo MIDI Type 1 exportado desde otro editor de partituras. Contiene 2 pistas: (a) Flauta — melodía en Sol mayor, 4/4, 32 compases, ámbito Sol₄–Mi₆, con ritmos de negra y corchea, perfectamente cuantizada. (b) Piano — acompañamiento en el gran pentagrama con acordes en redondas y blancas en la mano izquierda y arpegios simples en la mano derecha. El archivo DEBE incluir mensajes de Program Change correctos (Flute = program 73 o 74, Acoustic Grand Piano = program 1) y estar en formato Type 1 con las pistas separadas. NO debe tener errores de cuantización, notas superpuestas ni enarmonías extrañas. Es el "caso fácil".

2. **`ejercicio_S23_desastre.mid`**: Archivo MIDI Type 1 deliberadamente problemático. Debe contener: (a) microdesplazamientos rítmicos (notas grabadas en vivo sin cuantizar), (b) notas superpuestas en varios pasajes (simular pedal de piano mal utilizado), (c) armadura incorrecta o ausente (el MIDI no especifica tonalidad, la música está en Mi bemol mayor pero no hay mensaje de key signature), (d) enarmonías forzadas (varios Do♯ que deberían ser Re♭ en el contexto de Mi bemol mayor), (e) 3 pentagramas con nombres genéricos "Pista 1", "Pista 2", "Pista 3" siendo que los instrumentos reales son: violín, viola y violonchelo, (f) plicas inconsistentes en varios pasajes, (g) mensajes CC7 (volumen) que se convertirán en marcas de dinámica mal ubicadas. Duración: 24–32 compases. Debe ser reconocible como una pieza musical (no ruido aleatorio) para que los estudiantes puedan evaluar si la limpieza fue exitosa escuchando el resultado.

3. **`ejercicio_S23_karaoke.kar`**: Archivo .KAR con una canción popular en español (sugerencia: una balada o canción infantil con melodía clara y letra simple). Debe contener: pista de melodía (voz principal), pista de acompañamiento (piano o guitarra), y letra incrustada como eventos de letra MIDI. Incluir deliberadamente algunos caracteres de karaoke (/, -, _) que los estudiantes deban limpiar.

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Importar y diagnosticar el archivo limpio.
2. Limpiar el archivo problemático resolviendo ≥5 problemas.
3. Importar .KAR y corregir letra + agregar cifrado.
4. Buscar, importar y limpiar un archivo MIDI propio (Type 1, ≥4 instrumentos).
5. Reflexionar sobre cuándo importar vs. escribir desde cero.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Importación limpia | Parámetros justificados; diagnóstico completo de pentagramas, instrumentos, armadura | Diagnóstico parcial o sin justificación | Sin diagnóstico |
| Limpieza del desastre | ≥5 problemas identificados y resueltos; cuantización aplicada; enarmonías corregidas; resultado legible | 3–4 problemas resueltos | ≤2 problemas |
| Karaoke .KAR | Letra sincronizada y limpia; pentagramas nombrados; cifrado armónico | Letra importada con errores | Sin procesar |
| MIDI propio | Type 1, ≥4 instrumentos; limpieza documentada; mejoras agregadas (metadatos, dinámicas) | Importado pero limpieza parcial | No importado o tipo incorrecto |
| Reflexión | 3 respuestas con criterio técnico; comparación importar vs. escribir | 2 respuestas correctas | ≤1 respuesta |

---

## 4. Cierre — Importar es el 10%, limpiar es el 90%

### Revisión por parejas (8 min)

- Intercambiar el archivo `ejercicio_S23_desastre` limpio: "Reproducí la versión limpia del compañero. ¿Suena igual que el MIDI original? ¿La partitura es legible?"
- "¿Cuántos problemas encontró cada uno? ¿Coinciden? ¿Alguno encontró un problema que el otro no vio?" (Fomenta el aprendizaje de diagnóstico.)

### Puesta en común (7 min)

- "Levanten la mano los que encontraron que limpiar el desastre les llevó MÁS tiempo del que habrían tardado en escribirlo desde cero." (Estadística. Probablemente la mayoría.)
- "¿En qué momento decidirían 'esto no vale la pena, mejor lo escribo de nuevo'?" (Discusión sobre punto de quiebre: ¿40% de limpieza? ¿50%?)
- "¿Qué tipo de archivos MIDI les gustaría encontrar en internet para sus proyectos? ¿Cuáles evitarían?" (Discusión: preferir Type 1 sobre Type 0, MIDI de editores de partituras sobre grabaciones en vivo, archivos con nombres de pista descriptivos.)

### Resumen del docente (5 min)

1. **La importación MIDI es un borrador, no un producto final.** Lo que sale de la importación es el 10% del trabajo. El 90% es limpieza. Quien espera que "funcione solo" se va a decepcionar. Quien entiende que es un punto de partida, gana horas de trabajo.
2. **Los 7 problemas son predecibles.** Ritmos extraños, notas superpuestas, armaduras, enarmonías, pentagramas, plicas, dinámicas. No son "errores de MuseScore". Son consecuencias inevitables de traducir un protocolo de interpretación (MIDI) a un sistema de notación (partitura). Aprendan a diagnosticarlos rápido.
3. **MIDI de partitura = excelente. MIDI de grabación = problema.** La diferencia no está en MuseScore, está en el archivo fuente. Antes de importar, pregúntense: "¿este MIDI fue generado desde una partitura o desde una interpretación humana?" La respuesta define tu estrategia.
4. **La cuantización es tu bisturí, no tu martillo.** Usala con criterio. Demasiada = música robótica. Muy poca = caos. El punto justo depende del estilo y del tempo.
5. **A veces es más rápido escribir desde cero.** Un MIDI malo puede llevarte 45 minutos de limpieza. La misma partitura desde cero te lleva 30. Saber reconocer cuándo ABANDONAR un MIDI es tan importante como saber limpiarlo.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| El archivo MIDI no se abre o da error | Verificar que el archivo no esté corrupto. Probar abrirlo con otro programa (VLC, Windows Media Player, cualquier reproductor MIDI). Si otro programa lo abre, puede ser un problema de permisos de archivo o de ruta (evitar caracteres especiales o rutas muy largas). Si ningún programa lo abre, el archivo está dañado. |
| La importación genera 47 pentagramas para un archivo que debería tener 3 | El archivo probablemente es Type 0 (todas las pistas combinadas). Solución: buscar en internet "MIDI Type 0 to Type 1 converter" y convertir antes de importar. O aceptar la realidad y eliminar manualmente los pentagramas sobrantes. |
| Después de cuantizar, algunas notas desaparecen o se fusionan con silencios | La cuantización fue demasiado agresiva (ej. cuantizar a negra cuando hay corcheas). Deshacer (`Ctrl + Z`) y probar con una figura más pequeña (corchea → semicorchea). Si las notas cortas son esenciales, no cuantizar ese pasaje y corregir manualmente. |
| El estudiante no encuentra la opción de cuantización | Depende de la versión de MuseScore. En 4.x: está en **Herramientas → Cuantizar** o **Editar → Cuantización**. Si no aparece, buscar "quantize" en el manual. Si la versión no tiene cuantización nativa, el flujo alternativo es: exportar como MIDI desde MuseScore, abrir en un DAW, cuantizar allí, y reimportar. |
| Las enarmonías no cambian con `J` | `J` solo funciona en notas sueltas. Para cambios masivos: seleccionar todas las notas de un pasaje → clic derecho → **Propiedades de la nota → Alteración**. O usar **Herramientas → Respelling** (reescritura enarmónica automática). |
| La letra del .KAR está completamente desincronizada (3 sílabas de retraso) | Seleccionar toda la letra → `Ctrl + X` (cortar) → seleccionar la primera nota de la melodía → `Ctrl + V` (pegar). La letra se realinea desde el principio. Si la desincronización es variable (a veces adelantada, a veces atrasada), es problema del archivo .KAR original; corregir manualmente sílaba por sílaba. |
| El archivo MIDI suena bien pero la partitura se ve horrible (todo correcto auditivamente, visualmente un caos) | Este es el problema CONCEPTUAL más difícil de aceptar: MIDI y partitura tienen requisitos DIFERENTES. Un ritmo "correcto" en MIDI (una nota desplazada 30 ms) es ilegible en partitura. La limpieza NO preserva la fidelidad al MIDI original: preserva la LEGIBILIDAD. A veces hay que "mentir" en la partitura para que sea tocable por un humano. |
| El estudiante quiere importar un archivo MP3 o WAV (audio) como si fuera MIDI | DETENER inmediatamente. Explicar enfáticamente: "MIDI y audio son formatos INCOMPATIBLES. No podés 'importar' un MP3 como partitura. Es como querer convertir una foto de un perro en el perro real. Existen herramientas de audio-a-MIDI (como Melodyne, AnthemScore, o Basic Pitch de Spotify) pero son aproximaciones, no conversiones exactas." |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — MIDI import](https://handbook.musescore.org/advanced-topics/midi-import.md)
- [MuseScore Studio Handbook — File formats](https://handbook.musescore.org/basics/file-formats.md)
- **Preparación del archivo `ejercicio_S23_melodia.mid`**: la forma más rápida es crear la partitura directamente en MuseScore (Flauta + Piano en Sol mayor, 4/4, 32 compases) y luego exportar como MIDI (Archivo → Exportar → MIDI). Esto garantiza cuantización perfecta, asignación correcta de instrumentos y formato Type 1. Alternativamente, usar cualquier editor de partituras (Finale, Sibelius, Dorico) para generar el MIDI. NO usar grabaciones en vivo ni secuenciadores.
- **Preparación del archivo `ejercicio_S23_desastre.mid`**: la mejor estrategia es grabar una interpretación en vivo con un teclado MIDI (o pedir a un colega pianista que lo haga) y NO cuantizar. Tocar con pedal excesivo, con pequeñas imprecisiones rítmicas (rubato leve), en una tonalidad con bemoles (Mi bemol mayor) pero sin configurar la armadura en el secuenciador. Asignar instrumentos genéricos (pistas con nombres por defecto). Luego guardar como Type 1. El objetivo es que sea un archivo REALISTA, no una caricatura. Si no hay acceso a un teclado MIDI, se puede editar manualmente un archivo MIDI con un editor hexadecimal o un secuenciador para introducir los problemas deliberadamente.
- **Preparación del archivo `ejercicio_S23_karaoke.kar`**: descargar archivos .KAR desde repositorios de karaoke MIDI (sitios como midikar.com, vanBasco, etc.) o crear uno propio: escribir una melodía con letra en MuseScore (usando Lyrics `Ctrl + L`), exportar como MIDI Type 1 con letra, y renombrar la extensión a .KAR. MuseScore exporta la letra como metadatos MIDI que son reconocibles al reimportar. Verificar que la letra tenga algunos caracteres de karaoke (/, -, _) insertados manualmente para que los estudiantes practiquen la limpieza.
- Dato curioso: el formato MIDI fue diseñado en 1982–1983 por un comité de ingenieros de Sequential Circuits, Roland, Yamaha, Korg y Kawai. La primera canción en usar MIDI para sincronizar instrumentos fue el álbum *Thriller* de Michael Jackson (1982), donde usaron un precursor del MIDI para sincronizar sintetizadores. Para 1985, prácticamente todos los sintetizadores del mercado tenían puerto MIDI.
- Dato curioso: la razón por la que los archivos .KAR existen como formato separado es histórica. En los años 90, los fabricantes de máquinas de karaoke (principalmente japoneses) necesitaban una forma de incluir letra sincronizada en archivos MIDI sin romper el estándar. Extendieron el formato MIDI agregando eventos de texto con un esquema propietario. La extensión .KAR le dice al software "este archivo tiene letra, tratalo como karaoke". Técnicamente, un .KAR es un .MID con metadatos adicionales.
- Dato curioso: la limpieza de partituras MIDI es una habilidad profesional real. Los copistas y transcriptores musicales que trabajan para editoriales (Hal Leonard, Alfred Music, Boosey & Hawkes) frecuentemente reciben archivos MIDI de compositores o arregladores y deben convertirlos en partituras publicables. No es raro que un transcriptor profesional pase 4–6 horas limpiando un archivo MIDI de 10 minutos de música orquestal. Es un trabajo especializado que requiere conocimiento de notación, instrumentación y convenciones editoriales.
- Ejercicio opcional de ampliación (para estudiantes avanzados): entregar una carpeta con 10 archivos MIDI variados (Type 0, Type 1, .KAR, grabaciones en vivo, grabaciones cuantizadas, archivos de internet). Pedir a los estudiantes que CATEGORICEN cada archivo como "importable con poca limpieza", "importable con mucha limpieza", o "no importable (mejor escribir desde cero)", justificando cada categorización. Es un ejercicio de desarrollo de criterio profesional.

---

*Guía docente — Tecnología Musical I | Sesión 23*
