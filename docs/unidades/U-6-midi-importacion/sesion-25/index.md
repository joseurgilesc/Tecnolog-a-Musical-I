# Sesión 25: Reproducción como herramienta de revisión

📚 Handbook → Sound and Playback: Play mode, Synthesizer, Soundfonts | Herramientas: MuseScore Studio 4, Google Classroom, auriculares

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="play-mode"></a> **Modo de reproducción (Play mode)** | Uno de los tres modos principales de MuseScore (junto con Setup y Publish). En este modo se controla la reproducción de la partitura: iniciar, pausar, detener, avanzar, retroceder, ajustar tempo, activar loop. El panel de reproducción aparece en la parte superior de la ventana y es el "transporte" de MuseScore — análogo a los botones de un grabador de cinta. |
    | <a id="sintetizador"></a> **Sintetizador (Synthesizer)** | Motor interno de MuseScore que convierte las notas de la partitura en audio audible. NO es un sintetizador creativo (como los de música electrónica): es un reproductor de samples. Su función es tomar las notas escritas en el pentagrama, buscar el sonido correspondiente en el soundfont, aplicarle dinámicas y efectos, y enviar el audio resultante a los parlantes. |
    | <a id="soundfont"></a> **Soundfont (.sf2, .sf3)** | Archivo que contiene cientos o miles de grabaciones reales de instrumentos (samples). Cada nota de cada instrumento fue grabada individualmente y almacenada en el archivo. Cuando MuseScore necesita reproducir un Do₄ de violín, busca en el soundfont la grabación "Violín → Do₄ → mezzoforte" y la reproduce. Es como tener una orquesta grabada dentro de un archivo. |
    | <a id="ms-basic"></a> **MS Basic (MuseScore Basic)** | Soundfont por defecto de MuseScore 4. Es una versión reducida y optimizada de Muse Sounds. Incluye todos los instrumentos orquestales estándar (cuerdas, vientos, metales, percusión) y muchos instrumentos de banda y jazz. Está diseñado para ser funcional ocupando poco espacio (~100 MB). No tiene la calidad de Muse Sounds, pero es rápido y siempre funciona. |
    | <a id="muse-sounds"></a> **Muse Sounds** | Soundfont/librería de alta calidad de Muse Group. Incluye grabaciones profesionales de instrumentos orquestales, coros y banda. Requiere instalación separada (~2 GB) y más recursos de CPU. La diferencia es notable: legato real entre notas, vibrato natural, cambios de arco en cuerdas, staccato y pizzicato auténticos. Es el equivalente a "HD" para la reproducción de partituras. |
    | <a id="loop"></a> **Reproducción en bucle (Loop playback)** | Función que repite continuamente un fragmento seleccionado de la partitura. Esencial para revisar pasajes difíciles sin tener que hacer clic en "play" una y otra vez. Se activa seleccionando los compases deseados y presionando el botón de loop en el panel de reproducción, o con el atajo `;` (punto y coma). |
    | <a id="mixer"></a> **Mezclador (Mixer)** | Panel que muestra todos los instrumentos de la partitura con controles individuales de volumen (fader), panorama (izquierda/derecha), mute (silencio), solo (escuchar solo ese instrumento) y efecto de reverberación. Es el equivalente al mezclador de un estudio de grabación pero dentro de MuseScore. |
    | <a id="metronomo"></a> **Metrónomo (Metronome)** | Clic audible que marca el pulso durante la reproducción. Se activa/desactiva con el icono de metrónomo en el panel de reproducción. Indispensable para verificar que los ritmos escritos coinciden con el pulso real, especialmente en pasajes con tresillos, síncopas o cambios de compás. |
    | <a id="count-in"></a> **Conteo de entrada (Count-in)** | Opción que hace sonar uno o dos compases de clic ANTES de que empiece la reproducción. Permite "entrar a tiempo" mentalmente, como cuando un director levanta la batuta antes del primer compás. Se configura en **Reproducción → Configuración de reproducción → Conteo de entrada**. |
    | <a id="tempo-playback"></a> **Tempo de reproducción** | Velocidad a la que MuseScore reproduce la partitura, expresada en BPM (beats por minuto). El tempo por defecto es el indicado en la partitura (ej. ♩ = 120), pero puede modificarse temporalmente en el panel de reproducción sin alterar la indicación de tempo escrita. Esto permite ralentizar pasajes difíciles para revisarlos con detalle: "escucho la semicorchea del compás 47 a mitad de velocidad para ver si está bien escrita". |
    | <a id="cursor-reproduccion"></a> **Cursor de reproducción** | Línea vertical azul que avanza por la partitura durante la reproducción, indicando exactamente qué nota está sonando en cada momento. Al detener la reproducción, el cursor se queda en la última posición. Para reiniciar desde el principio: hacer clic en cualquier parte de la partitura y presionar `Ctrl + Inicio` o usar el botón "Ir al inicio". |
    | <a id="revision-auditiva"></a> **Revisión auditiva (auditory proofreading)** | Técnica de corrección que consiste en ESCUCHAR críticamente la reproducción de la partitura para detectar errores que el ojo pasa por alto. El cerebro procesa la música de manera diferente cuando la lee (visual) que cuando la escucha (auditiva). Errores como una alteración faltante, una nota equivocada en un acorde denso, o un ritmo mal transcrito son EVIDENTES al escuchar pero casi invisibles al leer. |
    | <a id="eq-reproduccion"></a> **EQ y efectos en reproducción** | MuseScore NO es un DAW, pero el mezclador incluye controles básicos de ecualización (graves, medios, agudos) por pista y un efecto de reverberación global. Estos NO afectan a la partitura impresa: son solo para mejorar la experiencia de escucha durante la reproducción. NO uses el EQ para "arreglar" una mala orquestación: si suena mal sin EQ, suena mal. |

???+ note "El panel de reproducción: tu tercer oído"

    La reproducción en MuseScore no es solo para "escuchar cómo suena". Es una HERRAMIENTA DE REVISIÓN tan importante como la vista. Los editores de partituras profesionales pasan casi tanto tiempo escuchando como escribiendo.

    ### Los controles esenciales

    El panel de reproducción (también llamado "transporte") está en la barra de herramientas superior. Sus controles principales:

    | Botón | Atajo | Función |
    |---|---|---|
    | ▶ **Reproducir** | `Espacio` | Inicia la reproducción desde el cursor. Si el cursor está al final, reinicia desde el principio. |
    | ⏸ **Pausar** | `Espacio` (durante reproducción) | Pausa. Al reanudar, continúa exactamente donde estaba. |
    | ⏹ **Detener** | `Escape` | Detiene y el cursor regresa a la posición donde empezó. |
    | ⏮ **Ir al inicio** | `Ctrl + Inicio` | Retrocede al primer compás sin reproducir. |
    | 🔄 **Loop** | `;` (punto y coma) | Activa/desactiva la reproducción en bucle del fragmento seleccionado. |
    | 🎵 **Metrónomo** | — | Activa/desactiva el clic del metrónomo durante la reproducción. |
    | ⏱ **Tempo** | — | Ajusta la velocidad temporalmente (no modifica la indicación de tempo en la partitura). |

    ### Reproducción selectiva

    No necesitás escuchar toda la sinfonía para revisar un compás. Métodos de reproducción parcial:

    1. **Desde un compás específico**: hacer clic en una nota o silencio → `Espacio`. La reproducción empieza exactamente desde ahí.
    2. **Desde un punto específico dentro del compás**: hacer clic en el tiempo deseado del compás → `Espacio`.
    3. **Solo un fragmento (loop)**: seleccionar el pasaje (clic en el primer compás, `Shift + clic` en el último) → `;` → `Espacio`. El fragmento se repite indefinidamente.
    4. **Solo un pentagrama**: en el mezclador (`F10`), hacer clic en **Solo** (S) en el instrumento deseado. Todos los demás se silencian temporalmente.

    ### Reproducción con conteo rítmico

    Para verificar ritmos complejos:
    1. Activar el metrónomo.
    2. Activar el conteo de entrada (1 o 2 compases previos).
    3. Reducir el tempo al 50–70% (usar el slider de tempo).
    4. Escuchar: "¿el ritmo que escribí coincide con el clic del metrónomo o se desfasa?"

    !!! tip "El loop es tu mejor amigo para pasajes difíciles"
        Nunca revises un pasaje complejo escuchándolo UNA SOLA VEZ. Ponelo en loop, reducí el tempo al 60%, cerrá los ojos, y escuchá 4 o 5 veces seguidas. La primera vez notás lo obvio (una nota que suena muy mal). La cuarta vez empezás a notar lo sutil (el balance entre voces, la articulación que no se aplicó, la dinámica que falta).

    > Insertar captura del panel de reproducción de MuseScore con los controles etiquetados y el loop activo sobre un fragmento seleccionado.

???+ note "El sintetizador y los soundfonts: qué suena y por qué"

    Cuando presionás "Play" en MuseScore, NO hay una orquesta escondida dentro de tu computadora. Lo que escuchás es el resultado de un proceso de dos pasos: (1) MuseScore lee las notas de la partitura, (2) el sintetizador busca los sonidos correspondientes en el soundfont.

    ### Cómo funciona un soundfont

    Un soundfont es una "caja de sonidos". Dentro hay:
    - **Muestras (samples)**: grabaciones reales de cada nota de cada instrumento. Un violín sampleado profesionalmente tiene grabaciones separadas para cada semitono en 3–4 niveles de dinámica (pp, mf, ff), con y sin vibrato, con diferentes articulaciones (arco, pizzicato, staccato, trémolo).
    - **Instrucciones**: reglas sobre cómo conectar las muestras. Por ejemplo: "cuando dos notas están ligadas, usá la muestra de legato en lugar de la muestra de ataque".

    ### MS Basic vs. Muse Sounds

    | Característica | MS Basic | Muse Sounds |
    |---|---|---|
    | **Tamaño** | ~100 MB | ~2 GB |
    | **Calidad de sonido** | Funcional, sintético en algunos registros | Profesional, cercano a librerías comerciales |
    | **Variedad de instrumentos** | Orquesta completa + banda y jazz | Orquesta completa + coros + banda |
    | **Legato entre notas** | Básico (conexión simple) | Real (transiciones grabadas entre intervalos) |
    | **Vibrato** | Artificial (generado por algoritmo) | Real (grabado por el instrumentista) |
    | **Cambios de arco / respiración** | Ausentes | Simulados |
    | **Uso de CPU** | Bajo (funciona en cualquier computadora) | Alto (requiere computadora con buen procesador) |
    | **¿Para qué sirve?** | Trabajo diario, esbozos, revisión rápida | Escucha crítica, entrega de audio, demo profesional |

    ### Instalar Muse Sounds

    1. Abrir MuseScore Studio.
    2. Ir a **Muse Hub** (el programa independiente que gestiona sonidos, no está dentro de MuseScore).
    3. En Muse Hub, ir a la pestaña **Sonidos**.
    4. Buscar "Muse Sounds" y hacer clic en **Instalar**.
    5. La descarga puede tomar tiempo (2 GB). Una vez instalado, reiniciar MuseScore.
    6. Al abrir una partitura, MuseScore usará Muse Sounds automáticamente si están disponibles.

    !!! info "Muse Hub"
        Muse Hub es una aplicación separada de MuseScore que funciona como "tienda" de sonidos, efectos y plugins gratuitos de Muse Group. Viene incluida con MuseScore 4 pero no se abre automáticamente. Debe ejecutarse manualmente al menos la primera vez para instalar los sonidos.

    ### Cambiar el soundfont de un instrumento

    Si querés que tu trompeta use un sonido diferente:
    1. Abrir el mezclador (`F10`).
    2. En la pista de Trompeta, hacer clic en el nombre del soundfont actual (ej. "MS Basic").
    3. Seleccionar "Muse Sounds" (si está instalado) o "Cambiar soundfont..." para cargar un archivo .sf2 o .sf3 personalizado.
    4. La asignación se guarda CON la partitura. Al compartir el .mscz, la otra persona necesitará el mismo soundfont instalado para escuchar lo mismo.

    ### Soundfonts de terceros

    Existen soundfonts gratuitos de alta calidad más allá de lo que ofrece Muse Group:
    - **FluidR3_GM.sf2** (141 MB): soundfont General MIDI completo, excelente relación calidad/tamaño. Muy usado en la comunidad de código abierto.
    - **TimGM6mb.sf2** (5.7 MB): tiny soundfont para sistemas con poca memoria. Calidad baja pero funcional.
    - **Timbres of Heaven** (340 MB): soundfont orientado a música de videojuegos y orquestal cinematográfico.
    - **Virtual Playing Orchestra**: soundfont de orquesta sinfónica creado por la comunidad, gratuito.

    Para cargar un soundfont personalizado en MuseScore: **Editar → Preferencias → Audio → Soundfont → Agregar**.

    !!! warning "Un soundfont NO es un sintetizador creativo"
        No podés "diseñar sonidos" con un soundfont. No tiene osciladores, filtros ni envolventes editables como un sintetizador (Vital, Serum, Sylenth1). El soundfont es un REPRODUCTOR de sonidos pregrabados. Si necesitás diseño sonoro creativo, exportá el MIDI a un DAW y usá sintetizadores reales.

    > Insertar captura del mezclador con la lista desplegable de soundfonts visibles para una pista, mostrando MS Basic, Muse Sounds y la opción "Cambiar soundfont...".

???+ note "La reproducción como herramienta de revisión crítica"

    Esta es la parte más importante de la sesión. La reproducción NO es entretenimiento. Es una MÁQUINA DE DETECTAR ERRORES.

    ### Lo que el oído detecta que el ojo ignora

    El ojo humano es excelente para reconocer patrones. Es TERRIBLE para detectar errores sutiles en esos patrones. Ejemplos reales:

    | Error | ¿El ojo lo ve? | ¿El oído lo detecta? |
    |---|---|---|
    | Escribiste Do♮ en un compás donde la armonía pide Do♯ | Depende. Si hay muchas alteraciones, el ojo asume que "está bien". | Inmediatamente. El Do♮ contra un acorde de La mayor (que tiene Do♯) suena HORRIBLE. |
    | Escribiste una negra en lugar de una corchea | Si el contexto es rítmicamente denso, difícil. | El oído detecta la inconsistencia rítmica al instante. |
    | La dinámica *p* está 2 pentagramas más abajo de donde debería | El ojo la ve pero no sabe si es intencional. | El oído escucha que un instrumento suena fuerte cuando debería sonar suave: inconsistencia. |
    | En un acorde de 4 voces, una voz tiene una nota duplicada incorrecta | Muy difícil de ver (hay que analizar cada voz por separado). | El oído detecta el "hueco" o la "disonancia extraña" en la textura. |
    | La ligadura de expresión cubre notas equivocadas | El ojo ve una curva sobre las notas y asume "correcto". | El oído escucha que las notas erróneas están ligadas incorrectamente. |
    | Un tresillo está mal escrito (2 corcheas en lugar de 3) | El ojo cuenta: "1, 2... sí, son 2". Pero ¿eran 3? | El oído detecta: "eso NO es un tresillo, es un ritmo binario". |

    ### El protocolo de revisión auditiva

    Sistema paso a paso para revisar una partitura usando la reproducción:

    **Paso 1: Escucha general (tempo real).**
    Reproducí la partitura completa a tempo de concierto. No te detengas. No corrijas nada todavía. Solo escuchá. Preguntate: ¿suena como la música que quería escribir? ¿La idea musical general está ahí? ¿Hay algo que "choque" fuertemente?

    **Paso 2: Escucha por instrumento (tempo real, un instrumento a la vez).**
    Usá el botón **Solo** en el mezclador para escuchar cada instrumento por separado. ¿La melodía es correcta? ¿El acompañamiento tiene sentido por sí mismo? ¿Las voces internas (viola, fagot, 2da trompeta) son lógicas o son "relleno"?

    **Paso 3: Escucha por pares (tempo reducido 70%).**
    Escuchá dos instrumentos a la vez (ej. melodía + bajo). ¿Las relaciones armónicas son correctas? ¿Hay choques de notas (segundas menores no intencionadas, octavas paralelas no deseadas)?

    **Paso 4: Escucha focalizada de pasajes difíciles (loop + tempo 50-60%).**
    Identificá los pasajes más complejos (cambios de compás, modulaciones, ritmos irregulares, contrapunto denso). Ponelos en loop a tempo reducido. Escuchá 5-6 veces. ¿Cada nota está en su lugar? ¿El ritmo es exacto? ¿Las alteraciones accidentales son correctas?

    **Paso 5: Escucha de transiciones (tempo real, últimos 2 compases de una sección + primeros 2 de la siguiente).**
    Las transiciones entre secciones son puntos críticos. Seleccioná 4 compases (2 antes + 2 después del cambio de sección) y reproducí. ¿La modulación es fluida? ¿El cambio de textura es natural? ¿El tempo se mantiene o hay indicación de cambio?

    ### Reglas de oro de la revisión auditiva

    1. **NUNCA confíes solo en tus ojos.** El oído encuentra lo que la vista normaliza.
    2. **Auriculares SÍ o SÍ.** Los parlantes de la laptop enmascaran errores. Con auriculares escuchás las voces internas, los roces entre notas, las desafinaciones sutiles.
    3. **Reducí el tempo para pasajes complejos.** Si no podés distinguir si una semicorchea está bien o mal a tempo real, reducí al 60% y escuchá. La nota incorrecta se vuelve OBVIA.
    4. **Escuchá CADA instrumento en solo al menos una vez.** Los errores en las voces internas son los más difíciles de detectar y los que más arruinan una partitura.
    5. **El metrónomo es tu juez rítmico.** Si escribiste un ritmo y no coincide con el clic del metrónomo, el ritmo está mal. No hay excusa: el metrónomo es matemáticamente exacto.
    6. **No te enamores de tu propio sonido.** Si algo suena mal, suena mal. No lo justifiques con "es que yo quería que sonara así". Corregilo.
    7. **Anotá TODO.** Durante la escucha, tené un papel (o un comentario de texto en MuseScore) para anotar: "c. 34, flauta, Fa debería ser Fa♯", "c. 56-58, ritmo de la viola no coincide con el metrónomo".

    !!! danger "El peligro de confiar solo en Muse Sounds"
        Muse Sounds es hermoso. Pero puede ENMASCARAR errores de orquestación. Un acorde mal espaciado en los metales suena "aceptable" con Muse Sounds pero sería IRREPRODUCIBLE por músicos reales. La reproducción de MuseScore es una aproximación, no una orquesta real. Si tu partitura va a ser tocada por humanos, la revisión auditiva es necesaria pero NO suficiente. Siempre complementá con análisis visual de los rangos instrumentales y las posibilidades técnicas reales.

    > Insertar captura del protocolo de revisión: pantalla dividida mostrando (1) el loop activo sobre un pasaje, (2) el mezclador con un instrumento en Solo, (3) el tempo reducido al 60%.

???+ note "El mezclador: balance y claridad"

    El mezclador (`F10`) es el panel de control maestro de la reproducción. Aunque no es un DAW profesional, ofrece herramientas esenciales para una revisión auditiva efectiva.

    ### Controles por pista

    Cada instrumento de la partitura aparece como una pista vertical con:

    | Control | Icono | Función |
    |---|---|---|
    | **Volumen (fader)** | Barra deslizante vertical | Ajusta el nivel de ese instrumento en la mezcla global. 0 = silencio, 100 = máximo. No afecta a la dinámica escrita (*p*, *f*): esos son valores RELATIVOS. |
    | **Panorama (pan)** | Perilla horizontal | Posiciona el instrumento en el espacio estéreo: izquierda, centro, derecha. Por defecto, los instrumentos se panoramizan automáticamente según su posición en la orquesta (violines I a la izquierda, chelos a la derecha). |
    | **Mute (M)** | Botón | Silencia completamente esa pista. El instrumento no se escucha pero sus notas siguen en la partitura. |
    | **Solo (S)** | Botón | Silencia TODAS las demás pistas y deja sonando solo esta. Útil para aislar un instrumento y revisarlo individualmente. |
    | **Reverb** | Perilla | Cantidad de reverberación (eco de sala) aplicada a ese instrumento. 0% = sonido seco (como en un estudio), más porcentaje = más ambiente de sala. |
    | **Soundfont** | Menú desplegable | Cambia el soundfont asignado a esa pista. |

    ### Ejercicio de escucha crítica con el mezclador

    1. Abrí una partitura de textura densa (orquesta, banda, ensamble de cámara).
    2. Activá **Solo** en el primer instrumento. Escuchá atentamente.
    3. Agregá el segundo instrumento (desactivá Solo del primero, activá Solo en ambos).
    4. ¿Se entiende cada línea? ¿Las voces se diferencian o se confunden?
    5. Si se confunden: ajustá el panorama (uno más a la izquierda, otro a la derecha) O ajustá el volumen relativo (melodía principal más fuerte, acompañamiento más suave) O — y esto es importante — **el problema puede ser de ORQUESTACIÓN, no de mezcla**. Si dos instrumentos tocan en el mismo registro con ritmos similares, ningún paneo ni volumen va a separarlos. La solución es REESCRIBIR, no mezclar.

    !!! tip "Un truco de editor profesional"
        Para verificar la independencia de las voces en una textura contrapuntística: silenciá TODOS los instrumentos menos dos. Escuchá la pareja. ¿Tiene sentido musical la conversación entre esos dos? Repetí con cada par posible. Si un instrumento no "dialoga" bien con NINGÚN otro, probablemente sobra.

    > Insertar captura del mezclador mostrando al menos 4 pistas con diferentes configuraciones de volumen, pan y reverb, y una pista en Solo.

---

## Actividad en Classroom

### Tarea: S25 — Reproducción como herramienta de revisión

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S25_errores.mscz`, una partitura de ensamble de vientos (flauta, oboe, clarinete en Si♭, fagot) de 40 compases, que contiene errores RÍTMICOS, ARMÓNICOS, DE ARTICULACIÓN y DE NOTACIÓN que DEBEN ser detectados auditivamente (no todos son visibles a simple vista); (b) `ejercicio_S25_mezcla.mscz`, una partitura para quinteto de cuerdas (violín I, violín II, viola, violonchelo, contrabajo) de 32 compases con un balance de mezcla deliberadamente malo, instrumentos con asignaciones incorrectas de soundfont y panoramización inadecuada.

1. **Detección de errores por reproducción.** Abrí `ejercicio_S25_errores.mscz` y NO mires la partitura todavía con intención de corregir. Primero, seguí el protocolo de revisión auditiva:
    - **Escucha general (tempo real, 1 vez)**: reproducí la partitura completa a tempo. Anotá tus primeras impresiones: ¿qué "choca"? ¿qué no suena como debería? ¿hay algo raro? (Mínimo 3 observaciones generales.)
    - **Escucha por instrumento (tempo real, 1 vez cada uno)**: usá Solo en cada instrumento (flauta, oboe, clarinete, fagot) y escuchá. Anotá al menos 2 problemas específicos detectados en CADA instrumento.
    - **Escucha por pares (tempo reducido 70%)**: combiná pares (flauta+oboe, clarinete+fagot, flauta+fagot, oboe+clarinete). Anotá problemas de relación entre instrumentos.
    - **Loop de pasajes sospechosos (tempo 50%)**: identificá los 3 pasajes más problemáticos y ponelos en loop a mitad de tempo. ¿Qué notas exactas están mal?
    - **Corrección**: una vez identificados TODOS los errores auditivamente, corregilos en la partitura. Guardá como `APELLIDO_Nombre_S25_errores_corregido.mscz`.

2. **Documentación del protocolo de revisión.** En Classroom, documentá tu proceso con la siguiente tabla para al menos 8 errores encontrados:

    | # | Compás(es) | Instrumento | Tipo de error (rítmico/armónico/articulación/notación) | ¿Era visible a simple vista? (Sí/No) | ¿Cómo lo detectaste auditivamente? |
    |---|---|---|---|---|---|
    | 1 | | | | | |
    | 2 | | | | | |
    | ... | | | | | |

3. **Mezcla y balance.** Abrí `ejercicio_S25_mezcla.mscz`:
    - La partitura tiene problemas de mezcla INTENCIONALES. Escuchá la reproducción completa y diagnosticá:
        - ¿Qué instrumento(s) está(n) demasiado fuerte(s)?
        - ¿Qué instrumento(s) apenas se escucha(n)?
        - ¿Está el panorama correcto? (violines I a la izquierda, violines II centro-izquierda, viola centro, violonchelo centro-derecha, contrabajo derecha)
        - ¿El soundfont asignado a cada instrumento es el correcto? (Un violín usando sonido de trompeta sería un error de asignación.)
    - Corregí: ajustá volúmenes en el mezclador, panoramizá correctamente, asigná los soundfonts correctos.
    - Guardá como `APELLIDO_Nombre_S25_mezcla_corregido.mscz`.

4. **Exploración de soundfonts.** Con la partitura corregida `APELLIDO_Nombre_S25_errores_corregido.mscz`:
    - Probá al menos DOS soundfonts diferentes para el mismo instrumento (ej. flauta con MS Basic vs. Muse Sounds, o clarinete con MS Basic vs. un soundfont alternativo que hayas instalado — FluidR3, Timbres of Heaven, o cualquier otro).
    - Compará: ¿cambia la calidad? ¿cambia la expresividad? ¿hay instrumentos que suenan mejor con un soundfont que con otro?
    - Escribí un párrafo de reflexión: "¿Qué soundfont prefiero para cada instrumento de este ensamble y por qué?".
    - Exportá la partitura como MP3 con:
        - Una versión usando SOLO MS Basic.
        - Una versión usando Muse Sounds (o el mejor soundfont alternativo que hayas instalado).
    - Nombrá los archivos: `APELLIDO_Nombre_S25_basic.mp3` y `APELLIDO_Nombre_S25_musesounds.mp3`.

5. **Reflexión sobre la revisión auditiva.** En Classroom, respondé:
    - ¿Encontraste errores que NO habías visto al leer la partitura pero que SÍ detectaste al escuchar? Describí al menos 2 ejemplos concretos.
    - ¿Creés que la revisión auditiva debería ser parte obligatoria de tu flujo de trabajo? ¿Por qué sí o por qué no? ¿Cuánto tiempo estimás que agrega al proceso de escritura de una partitura?
    - ¿Qué limitaciones tiene la revisión auditiva con MuseScore? ¿Qué tipo de errores NO podrías detectar solo escuchando la reproducción (y necesitás revisar visualmente)?

### Entregables

- [ ] `APELLIDO_Nombre_S25_errores_corregido.mscz`
- [ ] `APELLIDO_Nombre_S25_mezcla_corregido.mscz`
- [ ] `APELLIDO_Nombre_S25_basic.mp3`
- [ ] `APELLIDO_Nombre_S25_musesounds.mp3`
- [ ] Comentario en Classroom con: (a) tabla de 8+ errores con diagnóstico visual vs. auditivo, (b) diagnóstico y correcciones de mezcla, (c) comparación de soundfonts, (d) respuestas a las 3 preguntas de reflexión

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Detección de errores | ≥8 errores identificados auditivamente, documentados con tabla completa y corregidos en la partitura | 5–7 errores identificados | ≤4 errores o sin documentación |
| Protocolo de revisión | 5 pasos del protocolo aplicados sistemáticamente; notas de cada paso documentadas | 3–4 pasos aplicados | ≤2 pasos o aplicación superficial |
| Mezcla y balance | Volúmenes, pan y soundfonts corregidos; diagnóstico detallado documentado | Correcciones parciales | Sin correcciones |
| Comparación de soundfonts | 2+ soundfonts probados; comparación documentada; 2 MP3s exportados con nombres correctos | Un solo soundfont probado | Sin comparación |
| Reflexión | 3 respuestas con análisis de ejemplos concretos, justificación del uso de revisión auditiva y conciencia de limitaciones | 2 respuestas correctas | ≤1 respuesta o superficial |

---

*Basado en: MuseScore Studio 4 Handbook — Sound and Playback: Play mode, Synthesizer, Soundfonts | https://handbook.musescore.org*
