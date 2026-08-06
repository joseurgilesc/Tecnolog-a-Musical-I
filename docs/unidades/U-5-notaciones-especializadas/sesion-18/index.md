# Sesión 18: Notación de percusión

📚 Handbook → Notation: Entering and editing percussion notation, Noteheads | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="percusion-afinada"></a> **Percusión afinada (pitched percussion)** | Instrumentos de percusión que producen notas con altura definida: xilófono, marimba, vibráfono, glockenspiel, timbales, campanas tubulares. Se escriben en pentagramas normales (clave de Sol o Fa) y cada posición en el pentagrama representa una altura concreta. |
    | <a id="percusion-no-afinada"></a> **Percusión no afinada (unpitched percussion)** | Instrumentos que producen sonidos SIN altura definida: bombo, caja, platillos, triángulo, pandereta, castañuelas, woodblock. Se escriben en pentagramas especiales donde cada línea o espacio representa un instrumento diferente, no una nota musical. |
    | <a id="kit-bateria"></a> **Kit de batería (drum kit / drum set)** | Conjunto estándar de instrumentos de percusión no afinada tocados por un solo intérprete: bombo (kick), caja (snare), hi-hat, toms, platillos (crash, ride). En MuseScore, se configura como un solo pentagrama con una plantilla predefinida donde cada línea/espacio mapea a un tambor o platillo específico. |
    | <a id="mapa-percusion"></a> **Mapa de percusión (drum map / percussion map)** | Tabla que define qué sonido produce cada línea o espacio de un pentagrama de percusión. En MuseScore, al seleccionar "Drumset" como instrumento, se carga automáticamente el mapa estándar. Se puede personalizar desde **Editar → Preferencias → Percusión** (en versiones avanzadas) o desde el panel **Propiedades del pentagrama**. |
    | <a id="cabeza-nota"></a> **Cabeza de nota (notehead)** | Forma visual del símbolo de la nota. En notación estándar, la cabeza es ovalada (redonda, blanca, negra, etc.). En percusión, existen cabezas especiales: en X para platillos y hi-hat, triangular para pandereta, cuadrada para woodblock, diamante para armónicos, y circular normal para tambores. |
    | <a id="linea-platillo"></a> **Línea de platillo (cymbal line / ride line)** | En notación de batería, el hi-hat, ride y crash se escriben típicamente en las líneas superiores del pentagrama con cabezas en forma de X (o X con círculo para hi-hat abierto). La línea superior del pentagrama (por encima de la 5ª línea) suele reservarse para el ride, mientras que la línea por encima de esa (espacio superior) es para el crash. |
    | <a id="ghost-note"></a> **Nota fantasma (ghost note)** | En percusión (especialmente caja en batería), una nota tocada muy suavemente, casi inaudible, que añade textura rítmica. Se indica con una cabeza de nota entre paréntesis o con la indicación *ghost* como texto de pentagrama. En MuseScore, se puede lograr con una cabeza de nota más pequeña o con la dinámica *ppp*. |
    | <a id="redoble"></a> **Redoble (roll / diddle)** | Técnica de percusión donde se golpea el instrumento repetidamente a gran velocidad para crear un sonido sostenido. Se indica con una o más barras oblicuas sobre la plica. En MuseScore, se inserta desde la paleta **Articulaciones → Trémolo** o con líneas específicas de percusión. |
    | <a id="acento-percusion"></a> **Acento / Rimshot** | En percusión, un acento puede indicar un golpe fuerte (>), pero existe también el *rimshot* (golpe simultáneo al parche y al aro de la caja) que se indica con una cabeza especial o con la anotación "RS". Es uno de los sonidos más característicos de la caja en música popular. |
    | <a id="pedal-hi-hat"></a> **Hi-hat de pedal (pedal hi-hat)** | Sonido producido al cerrar el hi-hat con el pedal del pie izquierdo (sin usar baquetas). Se escribe como una X pequeña debajo del pentagrama o en la línea inferior. En MuseScore, corresponde a la nota F3 en el mapa estándar de batería (o a la línea de pedal hi-hat si está configurado). |
    | <a id="cross-stick"></a> **Cross-stick / Sidestick** | Técnica de caja donde se apoya la baqueta sobre el parche y se golpea el aro, produciendo un sonido seco similar a una clave. Se indica con una cabeza de nota en X colocada en la línea de la caja o con una cabeza especial. Es común en bossa nova, reggae y baladas. |
    | <a id="timbal"></a> **Timbal de orquesta (timpani)** | Instrumento de percusión afinada: tambores grandes (típicamente 2, 3 o 4) que pueden cambiar de afinación mediante un pedal. Se escriben en clave de Fa, con la nota indicando la altura afinada. Los cambios de afinación se indican con texto (*tune C to D*, *cambiar Fa a Sol*) o con glissandos si el cambio es durante la ejecución. |

???+ note "Percusión afinada: tímbales, xilófono y familia"

    La percusión afinada se escribe IGUAL que cualquier instrumento melódico: notas en un pentagrama con clave y armadura. La diferencia está en el TIMBRE, no en la notación.

    ### Instrumentos de percusión afinada y cómo se escriben

    | Instrumento | Clave | Ámbito típico | Particularidad en MuseScore |
    |---|---|---|---|
    | **Xilófono (xylophone)** | Sol | Fa₄–Do₇ (suena una octava arriba) | Es un instrumento transpositor: lo que escribís suena 1 octava MÁS AGUDA. Activá "altura de concierto" para verificar. |
    | **Marimba** | Sol (a veces Fa) | Do₃–Do₆ | No transpone. A menudo usa gran pentagrama (Sol arriba, Fa abajo) para cubrir todo el ámbito. |
    | **Vibráfono (vibraphone)** | Sol | Fa₃–Fa₆ | No transpone. Se escribe en un solo pentagrama de Sol. El efecto de trémolo/vibrato se indica con texto o con articulaciones de trémolo. |
    | **Glockenspiel** | Sol | Sol₄–Do₇ (suena DOS octavas arriba) | Altamente transpositor: suena 2 octavas arriba de lo escrito. MUCHO CUIDADO al exportar MIDI o al verificar con audio. |
    | **Campanas tubulares (chimes)** | Sol | Do₄–Fa₅ (suena como escrito) | Se escriben como notas normales. Los armónicos pueden indicarse con cabezas de diamante sobre la fundamental. |
    | **Timbales (timpani)** | Fa | 2–4 tambores: Re₂–La₃ típicamente | Cada tambor afina en una nota. Los cambios de afinación se indican con texto sobre el pentagrama (*Change D to C*, o *C → D*). NO se usa armadura (por tradición, las partituras de timbales omiten la armadura aunque la pieza esté en una tonalidad con sostenidos/bemoles). |

    ### Insertar percusión afinada en MuseScore

    1. Crear nueva partitura → seleccionar la familia **Percusión → Percusión afinada**.
    2. Elegir el instrumento: Xylophone, Marimba, Vibraphone, Glockenspiel, Timpani, etc.
    3. MuseScore configura automáticamente el pentagrama, la clave y la transposición (si corresponde).
    4. Ingresar notas normalmente con `N` y las letras del teclado. El sonido de reproducción corresponde al instrumento elegido.

    !!! warning "El xilófono y el glockenspiel TRANSPONEN"
        Este es el error más común al escribir para percusión afinada: no verificar la transposición. Un Do₄ escrito para glockenspiel suena como Do₆ real (DOS octavas arriba). Si tu partitura tiene otros instrumentos y el glockenspiel suena ridículamente agudo o desafinado, verificá la altura de concierto y la transposición. En MuseScore, el botón **Altura de concierto** (`Ctrl + Mayús + C` en algunas versiones) muestra las notas en su altura real.

    ### Timbales: el caso especial

    Los timbales merecen atención aparte porque:
    - **No llevan armadura de clave**: por convención, aunque la orquesta esté en Mi mayor (4 sostenidos), los timbales se escriben SIN armadura y todas las alteraciones son accidentales.
    - **Los cambios de afinación son texto**, no notas: `(C → D)` o `Change D to Eb` como Staff Text sobre el pentagrama.
    - **Glissando de timbal**: si el timbal cambia de afinación DURANTE la ejecución (con el pedal), se puede escribir un glissando entre las dos notas. MuseScore lo reproduce como un barrido de frecuencia.

    > Insertar captura de una partitura con timbales mostrando: ausencia de armadura, alteraciones accidentales, texto de cambio de afinación, y un glissando entre dos notas.

???+ note "Percusión no afinada: el pentagrama como mapa instrumental"

    En la percusión no afinada, el pentagrama NO representa alturas musicales. Cada línea y espacio es un "botón" que dispara un sonido diferente.

    ### El pentagrama de percusión: un mapa, no una escala

    | Posición en el pentagrama | Instrumento (mapa estándar batería) | Cabeza de nota |
    |---|---|---|
    | Encima de la 5ª línea | Crash (platillo) | X |
    | 5ª línea (superior) | Ride (platillo rítmico) | X |
    | Espacio sobre 4ª línea | Hi-hat abierto | X con círculo |
    | Espacio sobre 3ª línea | Hi-hat cerrado | X |
    | 3ª línea | Caja (snare) | Circular normal |
    | 1ª línea | Bombo (kick / bass drum) | Circular normal |
    | Debajo de la 1ª línea | Hi-hat de pedal | X pequeña |
    | 4ª línea / 2ª línea | Toms (agudo, medio, grave) | Circular normal |

    Este mapa NO es universal: cada editor y cada tradición (banda militar, orquesta, jazz) tiene pequeñas variaciones. MuseScore usa un mapa estándar basado en las convenciones de música popular y jazz.

    ### Cómo ingresar percusión no afinada en MuseScore

    1. Crear partitura → **Percusión → Percusión no afinada → Drumset (batería)**.
    2. El pentagrama aparece como una sola línea (no 5 líneas) por defecto. Podés cambiarlo a 5 líneas desde las Propiedades del pentagrama si preferís la notación de pentagrama completo.
    3. Activar modo de ingreso (`N`).
    4. **NO uses las letras A–G** para ingresar notas. En su lugar:
       - Hacé clic en la línea/espacio deseado con el mouse.
       - O usá el teclado MIDI si tenés uno conectado (cada tecla dispara un sonido del kit).
       - O usá las teclas de flecha ↑/↓ para mover la cabeza de nota entre líneas/espacios.
    5. La cabeza de nota cambia automáticamente según el instrumento (X para platillos, circular para tambores).

    !!! tip "El truco para memorizar el mapa de batería"
        Pensá en el pentagrama como una foto de la batería vista de frente: los platillos ARRIBA (agudos, metálicos), los tambores en el MEDIO, el bombo ABAJO (grave, el que se pisa). Cuanto más agudo es el sonido, más arriba se escribe. Es una metáfora física que ayuda a recordar.

    ### Escritura de patrones rítmicos básicos

    ```
    Compás 4/4, ritmo de rock básico:

    HH | x-x-x-x-x-x-x-x- |  (corcheas en hi-hat)
    SN | ----o-------o--- |  (caja en 2 y 4)
    BD | o-------o------- |  (bombo en 1 y 3)
    ```

    En MuseScore, escribís estas tres capas como VOCES diferentes dentro del mismo pentagrama de batería:
    - **Voz 1 (plica arriba)**: hi-hat y platillos (lo que toca la mano derecha).
    - **Voz 2 (plica abajo)**: caja y toms (lo que toca la mano izquierda + rellenos).
    - En algunos casos, **Voz 3** para el bombo (lo que toca el pie derecho), aunque normalmente el bombo comparte voz 1 o voz 2 con plicas hacia abajo.

    > Insertar captura de un pentagrama de batería con un patrón rítmico de 4 compases en estilo rock, mostrando las 3 capas (hi-hat voz 1 plica arriba, caja voz 2 plica abajo, bombo voz 2 plica abajo) con sus cabezas de nota correspondientes.

???+ note "Cabezas de nota especiales: el alfabeto visual de la percusión"

    En notación de percusión, la FORMA de la cabeza de nota comunica TANTA información como su posición en el pentagrama.

    ### Tipos de cabezas de nota y su significado

    | Cabeza | Forma | Uso en percusión | Atajo en MuseScore |
    |---|---|---|---|
    | **Normal (circular)** | ⚫ | Tambores: caja, bombo, toms, timbales | Default |
    | **X (cruz)** | ✕ | Platillos: hi-hat, ride, crash; también cross-stick en la caja | `Shift + X` (en algunas versiones) o paleta **Cabezas de nota** |
    | **X con círculo** | ⊕ | Hi-hat abierto, ride de campana (*bell*) | Paleta **Cabezas de nota** |
    | **Triángulo** | △ | Pandereta, triángulo (el instrumento), woodblock | Paleta **Cabezas de nota** |
    | **Diamante (rombo)** | ⬨ | Armónicos, campanas tubulares (nota fundamental con armónico), notas "fantasma" en vibráfono | Paleta **Cabezas de nota** |
    | **Cuadrado** | ⬛ | Woodblock, clave, cencerro (cowbell) en algunos estilos | Paleta **Cabezas de nota** |
    | **Paréntesis (ghost)** | (⚫) | Nota fantasma en caja (muy suave) | Propiedades → Tipo de cabeza → Parenthesized |
    | **Círculo pequeño** | ○ | Nota half-open (semiabierta) en hi-hat | Paleta **Cabezas de nota** |

    ### Cambiar la cabeza de una nota en MuseScore

    1. Seleccionar la nota.
    2. Ir a la paleta **Cabezas de nota** (Noteheads) en la zona de trabajo avanzado o desde **Ver → Paletas → Cabezas de nota**.
    3. Arrastrar la cabeza deseada sobre la nota, o hacer clic en la nueva cabeza.
    4. La nota cambia de forma pero mantiene su sonido original.

    O desde el panel **Propiedades → Nota → Tipo de cabeza**: seleccionar el tipo desde el desplegable.

    !!! warning "Cambiar la cabeza NO cambia el sonido"
        Si convertís una cabeza circular en X, la nota VA A SEGUIR SONANDO como el instrumento original mapeado a esa línea. La cabeza de nota es solo VISUAL. Para cambiar el sonido, necesitás mover la nota a otra línea/espacio en el pentagrama de percusión o cambiar el mapa de sonidos del pentagrama.

    ### Cabezas de nota y estilo de notación

    Algunos estilos musicales tienen convenciones diferentes:
    - **Jazz**: ride con cabeza de X, hi-hat con X, bombo con cabeza circular normal, caja con cabeza circular normal.
    - **Banda de concierto / Orquesta**: varios instrumentos de percusión pueden compartir un pentagrama con un mapa específico. Las cabezas ayudan a distinguir instrumentos: cuadradas para madera (woodblock), triangulares para metal (triángulo), X para platillos, circulares normales para tambores.
    - **Marching band (banda de marcha)**: cada tambor (caja, tenores, bombo) tiene su propio pentagrama individual. Las cabezas son todas circulares porque cada pentagrama representa un solo instrumento.

    > Insertar captura de la paleta **Cabezas de nota** en MuseScore mostrando todas las opciones: normal, X, X con círculo, triángulo, diamante, cuadrado, paréntesis, etc.

???+ note "Líneas y articulaciones para percusión"

    Además de las cabezas de nota, la notación de percusión usa líneas y símbolos especiales para indicar técnicas de ejecución.

    ### Redobles y trémolos

    Un redoble (roll) se indica con barras oblicuas sobre la plica de la nota:

    | Símbolo | Significado | Cómo insertarlo |
    |---|---|---|
    | Una barra oblicua | Redoble de corcheas (dos golpes por tiempo) | Paleta **Articulaciones → Trémolo** |
    | Dos barras oblicuas | Redoble de semicorcheas (cuatro golpes) | Paleta **Articulaciones → Trémolo** |
    | Tres barras oblicuas | Redoble de fusas (ocho golpes) | Paleta **Articulaciones → Trémolo** |
    | "Z" sobre la plica | *Buzz roll* (redoble presionado, usado en caja orquestal) | Paleta **Articulaciones** (buscar "buzz") o como texto |

    ### Acentos y articulaciones para percusión

    - **Acento normal (>)** : golpe fuerte.
    - **Marcato (^)** : golpe muy acentuado y separado.
    - **Staccato (.)** : golpe corto, especialmente en platillos (ahogar inmediatamente después del golpe).
    - **Tenuto (–)** : golpe con todo el valor, sin acortar.
    - **Fermata (𝄐)** : sostener el sonido (en platillos: dejar vibrar; en timbales: dejar resonar).

    ### Choke / Ahogar

    En platillos, el símbolo de **choke** (ahogar) indica que el sonido debe cortarse inmediatamente después del golpe (el percusionista agarra el platillo con la mano). Se indica con:
    - Un circulito con una cruz o una "c" pequeña sobre la nota.
    - La palabra *choke* o *ch.* como Staff Text.
    - En MuseScore, se puede simular acortando la duración de la nota del platillo y agregando un silencio inmediatamente después.

    > Insertar captura de un pasaje de percusión con: redoble de caja (doble barra oblicua), acentos en los golpes fuertes, choke en el crash, y un patrón de hi-hat con apertura/cierre.

---

## Actividad en Classroom

### Tarea: S18 — Notación de percusión

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S18_bateria.mscz`, un pentagrama de batería (drumset) en 4/4, 16 compases, completamente VACÍO (solo las líneas del pentagrama de percusión), listo para recibir patrones rítmicos; (b) `ejercicio_S18_timbales.mscz`, una partitura para timbales (2 tambores: Re₂ y La₂) en 3/4, 12 compases, con una melodía rítmica escrita pero SIN indicaciones de afinación ni cambios; (c) `ejercicio_S18_cabezas.mscz`, un pentagrama de percusión de 5 líneas con notas colocadas en diferentes posiciones pero TODAS con cabeza circular normal, requiriendo asignar las cabezas correctas según el instrumento mapeado.

1. **Patrones rítmicos de batería.** Abrí `ejercicio_S18_bateria.mscz`:
    - Activá el modo de ingreso (`N`) y familiarizate con el mapa de percusión: hacé clic en diferentes líneas/espacios para escuchar qué instrumento suena en cada posición.
    - **Patrón 1 — Rock básico** (c.1–4): hi-hat en corcheas (voz 1, cabeza de X), caja en tiempos 2 y 4 (voz 2, cabeza circular), bombo en tiempos 1 y 3 (voz 2, cabeza circular).
    - **Patrón 2 — Variación con fills** (c.5–8): mismo patrón base perο agregá fills de caja y toms en los compases 7–8 (semicorcheas moviéndose entre caja y toms agudo/medio/grave).
    - **Patrón 3 — Hi-hat con apertura** (c.9–12): usá hi-hat cerrado (cabeza X normal) para la mayor parte del patrón, pero abrí el hi-hat en el tiempo 4 de los compases 9 y 11 (cabeza X con círculo). Alterná entre cerrado y abierto.
    - **Patrón 4 — Ride y crash** (c.13–16): reemplazá el hi-hat por ride (cabeza X en la línea superior) para dar una sensación de "estribillo" más brillante. Agregá un crash (cabeza X encima de la 5ª línea) en el primer tiempo de los compases 13 y 15.
    - Reproducí todo el patrón de 16 compases. ¿Suena como una batería real tocando una canción?

2. **Timbales: afinación y cambios.** Abrí `ejercicio_S18_timbales.mscz`:
    - La partitura está en Re mayor (2 sostenidos). Verificá que los timbales NO tengan armadura de clave (si la tienen, eliminala seleccionando la armadura y presionando `Supr`).
    - Asegurate de que todas las alteraciones sean accidentales (sostenidos/bemoles escritos en cada nota, no heredados de una armadura invisible).
    - Insertá indicaciones de afinación como Staff Text (`Ctrl + T`) al inicio de la partitura: `Timpani in D, A` (los dos tambores afinados en Re₂ y La₂).
    - Localizá los compases donde el compositor pide un cambio de afinación (indicado con texto en la partitura: *change D to C* o similar). Insertá el texto correspondiente.
    - Si hay un cambio de afinación durante un silencio del timbalista, simulá un glissando: escribí la nota de partida, una línea de glissando (paleta **Líneas → Glissando**), y la nota de llegada. Aunque los timbales no hacen un glissando "real" (cambian la afinación con el pedal), la notación moderna acepta el glissando como indicación de cambio suave.

3. **Cabezas de nota: el alfabeto visual.** Abrí `ejercicio_S18_cabezas.mscz`:
    - El archivo tiene un pentagrama de percusión con el siguiente mapa (indicado en un recuadro de texto al inicio de la partitura):
      - Línea 3 (central): Caja (snare) → cabeza circular.
      - Espacio sobre línea 4: Hi-hat cerrado → cabeza X.
      - Espacio sobre línea 5: Hi-hat abierto → cabeza X con círculo.
      - 1ª línea: Bombo (kick) → cabeza circular.
      - 5ª línea: Ride → cabeza X.
      - Encima de 5ª línea: Crash → cabeza X.
      - Línea 2: Tom medio → cabeza circular.
      - Espacio sobre línea 3: Tom agudo → cabeza circular.
    - Todas las notas actualmente tienen cabeza circular. TU trabajo es asignar la cabeza correcta a cada nota según el instrumento que representa:
      - Seleccioná cada nota → Paleta **Cabezas de nota** → arrastrar la cabeza correspondiente.
    - Después de asignar todas las cabezas, verificá: ¿se entiende visualmente qué instrumento es cada uno sin necesidad de escuchar?

4. **Redobles y articulaciones de percusión.** En el mismo archivo `ejercicio_S18_bateria.mscz` ya editado:
    - Agregá un **redoble de caja** (doble barra oblicua sobre la plica) en el compás 16: una redonda con redoble que crezca hacia el final (agregá un regulador de crescendo debajo).
    - Agregá **acentos** (`>`) en los golpes de crash de los compases 13 y 15.
    - Agregá un **choke** (ahogar) en el crash del compás 15: escribí la palabra *choke* como Staff Text sobre la nota, y acortá la duración de la nota del crash (convertila en corchea en lugar de negra, dejando silencio el resto del tiempo).
    - Agregá una indicación de **cross-stick** en la caja en los compases 4 y 12: cambiá la cabeza de esas notas de caja a X (cruz) y escribí *cross-stick* como Staff Text sobre la primera ocurrencia.
    - Reproducí. ¿Los redobles se escuchan? ¿Los acentos se notan? ¿El choke corta el sonido?

5. **Integración: sección de percusión para ensamble.** Creá una NUEVA partitura desde cero: `APELLIDO_Nombre_S18_percusion.mscz`.
    - Plantilla: **Drumset (batería)** + **Timpani** + un instrumento de percusión afinada a elección (xilófono, marimba o vibráfono). Total: 3 pentagramas.
    - Tonalidad: La menor (sin armadura). Compás: 4/4. 32 compases.
    - **Batería** (pentagrama 1): Creá un patrón rítmico en 4 secciones:
      - A (c.1–8): ritmo de rock básico (hi-hat corcheas, caja en 2 y 4, bombo en 1 y 3).
      - B (c.9–16): variación con ride en lugar de hi-hat, crash en los inicios de sección.
      - C (c.17–24): ritmo más complejo: hi-hat con semicorcheas, síncopas en la caja y el bombo.
      - D (c.25–32): redoble de caja en los últimos 2 compases + crash con choke final.
    - **Timbales** (pentagrama 2): Escribí una parte de timbales usando 3 tambores: La₂, Re₃, Mi₃ (cambios de afinación indicados con texto). Usá redondas y blancas para crear una base armónica. SIN armadura de clave.
    - **Percusión afinada** (pentagrama 3): Componé una melodía sencilla en La menor pentatónica (La-Do-Re-Mi-Sol) usando corcheas y negras. Si elegiste xilófono o glockenspiel, verificá la transposición.
    - **Cabezas de nota**: en la batería, usá cabezas X para platillos, circulares para tambores, X con círculo para hi-hat abierto. Al menos 3 compases deben tener hi-hat abierto.
    - **Articulaciones**: agregá acentos en la caja (≥4), un redoble en el pentagrama de percusión afinada (trémolo entre dos notas), y dinámicas (*mf*, *f*, crescendo).
    - Exportá como PDF.

6. **Reflexión sobre notación de percusión.** En Classroom, respondé:
    - ¿Por qué la percusión no afinada no usa armadura de clave ni notas con altura definida? ¿Qué limitaciones tendría escribir un bombo como "Do" y una caja como "Re"?
    - ¿En qué se diferencia escribir para timbales de escribir para xilófono? Mencioná al menos 3 diferencias concretas (clave, armadura, transposición, notación de cambios, etc.).
    - Si tuvieras que inventar un símbolo nuevo para un instrumento de percusión que NO está en MuseScore (por ejemplo, un "cajón peruano" con diferentes zonas de golpe), ¿cómo lo representarías en el pentagrama? Describí tu propuesta de mapa y cabezas.

### Entregables

- [ ] `APELLIDO_Nombre_S18_bateria_v01.mscz` (batería con 4 patrones + redobles y articulaciones)
- [ ] `APELLIDO_Nombre_S18_bateria_v01.pdf`
- [ ] `APELLIDO_Nombre_S18_timbales_v01.mscz` (timbales con afinación y cambios)
- [ ] `APELLIDO_Nombre_S18_timbales_v01.pdf`
- [ ] `APELLIDO_Nombre_S18_cabezas_v01.mscz` (cabezas de nota asignadas correctamente)
- [ ] `APELLIDO_Nombre_S18_cabezas_v01.pdf`
- [ ] `APELLIDO_Nombre_S18_percusion_v01.mscz` (sección de percusión completa)
- [ ] `APELLIDO_Nombre_S18_percusion_v01.pdf`
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) breve descripción de cómo distribuiste las voces en la batería (qué instrumentos van en voz 1, cuáles en voz 2, y por qué)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Patrones de batería | 4 patrones completos y distintos; voces correctamente asignadas; hi-hat, caja, bombo y platillos en sus posiciones correctas | 3 patrones o alguna asignación incorrecta de voces/posiciones | ≤2 patrones o mapa de batería incorrecto |
| Timbales | Sin armadura; alteraciones accidentales; indicaciones de afinación presentes; cambios de afinación correctos | Timbales escritos pero con armadura o sin indicaciones de afinación | Timbales con errores graves (armadura, sin cambios) |
| Cabezas de nota | ≥90% de las cabezas asignadas correctamente según el mapa; X para platillos, circular para tambores | 70–89% correctas o algunas confusiones | <70% correctas o sin cambios |
| Redobles y articulaciones | Redoble correcto (barras oblicuas); acentos en crash; choke indicado; cross-stick con cabeza X | Redobles y articulaciones presentes pero con algún error | Sin redobles ni articulaciones |
| Sección de percusión integrada | 3 pentagramas completos; patrones A-B-C-D en batería; timbales correctos; melodía en percusión afinada; cabezas y articulaciones variadas | Faltan 1–2 elementos de la lista | ≥3 elementos faltantes o sección incompleta |
| Reflexión | Responde las 3 preguntas con comprensión de los conceptos; demuestra entender la diferencia entre percusión afinada y no afinada | Responde 2 de 3 correctamente | ≤1 respuesta correcta o superficial |

---

*Basado en: MuseScore Studio 4 Handbook — Entering and editing percussion notation, Noteheads | https://handbook.musescore.org*
