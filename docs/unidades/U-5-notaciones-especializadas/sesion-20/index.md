# Sesión 20: Transposición y escritura para instrumentos transpositores

📚 Handbook → Notation: Transposition | Sound and playback: Concert pitch | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="transposicion"></a> **Transposición (transposition)** | Proceso de cambiar la altura de una nota, pasaje o pieza completa a otra tonalidad sin alterar las relaciones interválicas. En este curso, "transposición" también se refiere a la práctica de escribir las notas de ciertos instrumentos en una altura DIFERENTE a la que realmente suenan. |
    | <a id="instrumento-transpositor"></a> **Instrumento transpositor (transposing instrument)** | Instrumento cuyo sonido real NO coincide con lo escrito en la partitura. Si escribís un Do en el pentagrama, el instrumento produce otra nota. Ejemplos: clarinete en Si♭ (suena Si♭ cuando leés Do), trompa en Fa (suena Fa cuando leés Do), saxofón alto en Mi♭ (suena Mi♭ cuando leés Do). |
    | <a id="tono-concierto"></a> **Tono de concierto (concert pitch)** | La altura REAL que suena. Cuando el director ve la partitura general (full score) en tono de concierto, todos los instrumentos muestran las notas que EFECTIVAMENTE se escuchan, sin transposición. Es la vista "objetiva" de la partitura. |
    | <a id="tono-escrito"></a> **Tono escrito (written pitch)** | La altura que el instrumentista LEE en su partitura individual. Para instrumentos no transpositores (piano, flauta, violín), tono escrito = tono de concierto. Para instrumentos transpositores, el tono escrito difiere del tono de concierto según la transposición del instrumento. |
    | <a id="armadura"></a> **Armadura de clave (key signature)** | En instrumentos transpositores, la armadura también se transpone. Si la pieza está en Do mayor (sin alteraciones) para piano, el clarinete en Si♭ leerá Re mayor (2 sostenidos) para que suene Do mayor. Cada familia de instrumentos tiene su propia armadura escrita. |
    | <a id="transposicion-cromatica"></a> **Transposición cromática (chromatic transposition)** | Transposición donde cada nota se mueve un número fijo de semitonos. Ejemplo: transponer todo +2 semitonos convierte Do→Re, Mi→Fa♯, Sol→La. Es lo que hace MuseScore cuando cambiás la tonalidad de una pieza completa. |
    | <a id="transposicion-diatonica"></a> **Transposición diatónica (diatonic transposition)** | Transposición donde las notas se mueven un número fijo de GRADOS de la escala (no semitonos), manteniendo las alteraciones dentro de la tonalidad de destino. Ejemplo: subir un grado en Do mayor mueve Do→Re, Mi→Fa, Sol→La, pero Mi→Fa es solo un semitono mientras que Do→Re es un tono entero. |
    | <a id="intervalo-transposicion"></a> **Intervalo de transposición** | La distancia entre el tono escrito y el tono de concierto para un instrumento transpositor. Se mide desde Do escrito hasta la nota que suena. Clarinete en Si♭: intervalo = 2ª mayor descendente (Do escrito → Si♭ sonando). Trompa en Fa: intervalo = 5ª justa descendente (Do escrito → Fa sonando). Saxofón alto en Mi♭: intervalo = 6ª mayor descendente (Do escrito → Mi♭ sonando). |
    | <a id="transposicion-octava"></a> **Transposición de octava** | Caso especial de transposición donde la diferencia es exactamente una octava (o múltiplos). Ejemplos: guitarra (suena 8ª baja), flautín/piccolo (suena 8ª alta), contrabajo (suena 8ª baja). Se indica con un pequeño "8" sobre o bajo la clave. |
    | <a id="clarinete-sib"></a> **Clarinete en Si♭** | El instrumento transpositor más común en bandas escolares y orquestas de viento. Cuando el clarinetista lee Do, suena Si♭ (un tono entero más bajo). Para que suene Do de concierto, debe leer Re. Suena una 2ª mayor por DEBAJO de lo escrito. |
    | <a id="trompa-fa"></a> **Trompa en Fa (French horn in F)** | Instrumento de la orquesta sinfónica. Cuando el cornista lee Do, suena Fa (una 5ª justa más baja). Es decir, suena una 5ª justa por DEBAJO de lo escrito. La trompa es uno de los instrumentos transpositores más "lejanos" respecto al tono escrito. |
    | <a id="saxofon-mib"></a> **Saxofón alto en Mi♭ / Saxofón barítono en Mi♭** | Suena una 6ª mayor por DEBAJO de lo escrito (alto) o una 6ª mayor + 8ª por debajo (barítono). El saxofón tenor en Si♭ suena una 9ª mayor (8ª + 2ª mayor) por debajo de lo escrito. |
    | <a id="trompeta-sib"></a> **Trompeta en Si♭** | La trompeta estándar actual. Suena una 2ª mayor por DEBAJO de lo escrito (igual que el clarinete). La trompeta en Do (menos común) es no transpositora. En partituras de orquesta, las partes de trompeta pueden aparecer en Do, Si♭, Re, Mi♭ o Fa según la época y tradición. |
    | <a id="partitura-general"></a> **Partitura general / Full score** | La partitura que contiene TODOS los instrumentos de la obra, cada uno en su propio pentagrama. En la tradición moderna, la partitura general puede mostrarse en tono de concierto (todos los instrumentos muestran lo que suena) o en tono escrito (cada instrumento muestra lo que su músico lee). MuseScore permite alternar entre ambas vistas con un solo clic. |

???+ note "¿Por qué existen los instrumentos transpositores?"

    Esta es una de las preguntas más frecuentes —y más mal respondidas— en la enseñanza musical. La respuesta real tiene TRES razones históricas y prácticas.

    ### 1. Familias de instrumentos que comparten digitación

    Un saxofonista que aprendió digitación en saxofón alto en Mi♭ puede tomar un saxofón tenor en Si♭, leer la misma partitura, usar los MISMOS dedos, y producir la melodía correcta... aunque suene en otra tonalidad. Si las partituras estuvieran en tono de concierto, el saxofonista tendría que aprender una digitación completamente diferente para CADA tamaño de saxofón.

    **Ejemplo concreto**: La escala de Do mayor escrita se toca con digitación idéntica en saxofón soprano (Si♭), alto (Mi♭), tenor (Si♭) y barítono (Mi♭). En los cuatro instrumentos, los dedos son los mismos. Lo que cambia es qué nota SALE: en el alto sale Mi♭ mayor, en el tenor sale Si♭ mayor. Pero el SAXOFONISTA NO PIENSA EN ESO. Lee Do, digita Do, y el instrumento hace su magia.

    !!! tip "La analogía del capo de guitarra"
        Si ponés un capo en el traste 2 de la guitarra y tocás los mismos acordes de siempre (Do, Sol, Lam), ESTÁS TRANSPONIENDO. Tus dedos hacen lo de siempre, pero suena un tono más alto. Los instrumentos transpositores tienen el "capo incorporado" por construcción.

    ### 2. Tradición orquestal del siglo XVIII-XIX

    Antes de la invención del pistón (válvula) en 1815, las trompas y trompetas eran "naturales": solo podían tocar los armónicos de una fundamental fija. Si la obra estaba en Re mayor, el cornista usaba una trompa en Re (con un tubo adicional o "tonillo" que cambiaba la fundamental). La parte se escribía SIEMPRE en Do mayor (sin alteraciones), independientemente de qué tonillo usara el instrumento. El compositor especificaba "Trompa en Re", "Trompa en Mi♭", etc., y el cornista leía todo como si estuviera en Do.

    Esta tradición SOBREVIVIÓ a la invención de la trompa cromática moderna. Hoy la trompa doble en Fa/Si♭ puede tocar cualquier nota, pero las partes se siguen escribiendo en Fa por INERCIA HISTÓRICA.

    ### 3. Lectura facilitada: evitar líneas adicionales

    Si las partes de flautín (piccolo) se escribieran en tono de concierto, el tercio superior del registro estaría PLAGADO de líneas adicionales. Al escribir una octava más baja de lo que suena, las notas caen cómodamente dentro del pentagrama. Lo mismo aplica al contrabajo y la guitarra en el extremo grave.

    | Instrumento | Tono escrito | Tono de concierto | Razón de la transposición |
    |---|---|---|---|
    | Flautín (piccolo) | Do₅–Do₇ | Do₆–Do₈ | Evitar líneas adicionales superiores (transposición de 8ª) |
    | Contrabajo | Do₂–Do₄ | Do₁–Do₃ | Evitar líneas adicionales inferiores (transposición de 8ª) |
    | Guitarra | Do₃–Do₅ | Do₂–Do₄ | Evitar cambio de clave (transposición de 8ª) |
    | Clarinete en Si♭ | Re₃–Sol₅ | Do₃–Fa₅ | Familia de instrumentos: misma digitación |
    | Saxofón alto en Mi♭ | Si♭₂–Fa₅ | Re♭₃–La₄ | Familia de instrumentos: misma digitación |
    | Trompa en Fa | Fa♯₂–Do₅ | Si₁–Fa₄ | Tradición histórica (trompa natural) |
    | Trompeta en Si♭ | Fa♯₃–Do₅ | Mi₃–Si♭₄ | Familia de instrumentos + tradición |

    > Insertar diagrama de los instrumentos transpositores más comunes con su intervalo de transposición respecto al Do escrito.

???+ note "Transposición en MuseScore: tres formas de transponer"

    MuseScore ofrece tres mecanismos diferentes de transposición. Es FUNDAMENTAL entender cuándo usar cada uno, porque hacen cosas DISTINTAS y confundirlos es la fuente #1 de errores de principiante.

    ### 1. Cambio de tonalidad (transposición diatónica)

    **Ruta**: Herramientas → Transponer... (o clic derecho en un pasaje seleccionado → Transponer...)

    **Qué hace**: Mueve todas las notas una cantidad fija de semitonos o a una nueva tonalidad, ajustando las alteraciones para mantener las relaciones diatónicas.

    **Cuándo usarlo**:
    - Querés cambiar la tonalidad de una pieza completa ("esto está en Do, pasalo a Re").
    - Querés transportar una melodía a un registro más cómodo para un cantante.
    - Necesitás adaptar un acompañamiento a la tesitura de un solista.

    **Ejemplo paso a paso**:
    1. Seleccioná toda la partitura (`Ctrl + A`).
    2. Herramientas → Transponer...
    3. Elegí "Por intervalo" y seleccioná, por ejemplo, "2ª mayor ascendente" para subir un tono entero.
    4. O elegí "A una tonalidad" y seleccioná la nueva tonalidad de destino.
    5. Marcá "Transponer armaduras de clave" si querés que la armadura también cambie.
    6. Aceptar.

    !!! warning "Cuidado con las notas fuera de rango"
        Si transponés una pieza para piano 2 octavas arriba, muchas notas van a quedar fuera del teclado o sonar ridículamente agudas. Siempre verificá el rango del instrumento después de transponer.

    ### 2. Configuración del instrumento (transposición de staff)

    **Ruta**: Propiedades del pentagrama (clic derecho en el pentagrama) → Transposición

    **Qué hace**: Define la transposición INHERENTE al instrumento. No modifica las notas visibles; modifica cómo se INTERPRETAN al reproducir.

    **Cuándo usarlo**:
    - Acabás de agregar un instrumento transpositor (clarinete, trompa, saxofón) y querés que MuseScore maneje automáticamente la diferencia entre tono escrito y tono de concierto.
    - Estás creando una partitura desde cero y necesitás configurar correctamente los instrumentos.
    - Cambiaste el instrumento de un pentagrama (ej. de flauta a clarinete) y necesitás actualizar la transposición.

    **Ejemplo paso a paso**:
    1. Clic derecho en el pentagrama del clarinete → Propiedades del pentagrama/parte...
    2. En la pestaña "Pentagrama", sección "Transposición":
       - "Transposición" → establecer el intervalo. Para clarinete en Si♭: "2ª mayor descendente".
       - "Suena" → marcar "una 2ª mayor más bajo de lo escrito".
    3. Aceptar. MuseScore ahora sabe que este pentagrama es un clarinete en Si♭ y aplica la transposición automáticamente.

    ### 3. Toggle de tono de concierto

    **Ruta**: Botón "Tono de concierto" en la barra de herramientas de reproducción (o menú Vista → Tono de concierto).

    **Qué hace**: NO transpone nada. Simplemente cambia lo que VES en pantalla:
    - **Activado** (tono de concierto): Todos los instrumentos muestran las notas en su altura REAL de sonido.
    - **Desactivado** (tono escrito): Los instrumentos transpositores muestran las notas que su MÚSICO LEE.

    **Analogía**: Es como un interruptor de idioma en un menú de restaurant. La comida es la misma, pero la ves en español o en inglés. Las notas NO cambian en el archivo, solo la visualización.

    **Cuándo usar cada vista**:
    - **Tono de concierto ACTIVADO**: cuando estás COMPONIENDO o ARREGLANDO. Querés ver y escuchar las alturas reales. Es la vista "objetiva" del director y el compositor.
    - **Tono escrito ACTIVADO**: cuando estás PREPARANDO PARTES para imprimir. Querés ver exactamente lo que cada músico va a leer en su atril.

    !!! tip "Regla de oro"
        Componé SIEMPRE en tono de concierto. Imprimí SIEMPRE en tono escrito. Si componés en tono escrito, vas a escribir acordes que no existen, armonías incorrectas, y notas fuera de rango sin darte cuenta.


???+ note "Los instrumentos transpositores uno por uno"

    ### Familia de los clarinetes y saxofones (familia Si♭/Mi♭)

    La transposición más común que vas a encontrar. Regla nemotécnica:

    | Instrumento | Tono escrito (leés Do) | Tono de concierto (suena) | Intervalo | Armadura escrita (si la pieza está en Do Mayor) |
    |---|---|---|---|---|
    | **Clarinete en Si♭** | Do | Si♭ | 2ª mayor ↓ | Re Mayor (2 ♯) |
    | **Clarinete bajo en Si♭** | Do | Si♭ (8ª abajo) | 9ª mayor ↓ | Re Mayor (2 ♯) |
    | **Saxofón soprano en Si♭** | Do | Si♭ | 2ª mayor ↓ | Re Mayor (2 ♯) |
    | **Saxofón tenor en Si♭** | Do | Si♭ (8ª abajo) | 9ª mayor ↓ | Re Mayor (2 ♯) |
    | **Saxofón alto en Mi♭** | Do | Mi♭ | 6ª mayor ↓ | La Mayor (3 ♯) |
    | **Saxofón barítono en Mi♭** | Do | Mi♭ (8ª abajo) | 6ª mayor + 8ª ↓ | La Mayor (3 ♯) |
    | **Clarinete en Mi♭ (requinto)** | Do | Mi♭ | 3ª menor ↑ | La♭ Mayor (4 ♭) |
    | **Clarinete en La** | Do | La | 3ª menor ↓ | Mi♭ Mayor (3 ♭) |

    !!! tip "Truco de armaduras"
        Para instrumentos en Si♭: la armadura escrita tiene **2 sostenidos MÁS** (o 2 bemoles MENOS) que la armadura de concierto. Do Mayor concierto (0 alteraciones) → Re Mayor escrito (2 ♯). Fa Mayor concierto (1 ♭) → Sol Mayor escrito (1 ♯). Mi♭ Mayor concierto (3 ♭) → Fa Mayor escrito (1 ♭).

        Para instrumentos en Mi♭: **3 sostenidos MÁS**. Do Mayor concierto → La Mayor escrito (3 ♯). Fa Mayor concierto (1 ♭) → Re Mayor escrito (2 ♯).

    ### Familia de las trompas y trompetas

    | Instrumento | Tono escrito | Tono de concierto | Intervalo |
    |---|---|---|---|
    | **Trompa en Fa** | Do | Fa | 5ª justa ↓ |
    | **Trompeta en Si♭** | Do | Si♭ | 2ª mayor ↓ |
    | **Trompeta en Do** | Do | Do | (no transpone) |
    | **Trompeta piccolo en Si♭** | Do | Si♭ (8ª arriba) | 7ª menor ↓ (es decir, suena más agudo que la trompeta normal) |
    | **Corneta en Si♭** | Do | Si♭ | 2ª mayor ↓ |
    | **Fliscorno (flugelhorn) en Si♭** | Do | Si♭ | 2ª mayor ↓ |

    !!! warning "La trompa NO transpone como el clarinete"
        Error clásico de principiante: asumir que "transpositor en Si♭/Fa" significa lo mismo para todos. La trompa en Fa NO es un instrumento en Si♭. La armadura para trompa en Fa en Do Mayor concierto es Sol Mayor (1 ♯), no Re Mayor. Cada familia tiene su PROPIA transposición.

    ### Familia de transposición de octava

    | Instrumento | Tono escrito | Tono de concierto | Indicación |
    |---|---|---|---|
    | **Flautín (piccolo)** | Do₄–Do₆ | Do₅–Do₇ | 8ª alta (8va sobre la clave) |
    | **Guitarra** | Do₃–Do₅ | Do₂–Do₄ | 8ª baja (8vb bajo la clave) |
    | **Contrabajo** | Do₂–Do₄ | Do₁–Do₃ | 8ª baja |
    | **Bajo eléctrico** | Do₂–Do₄ | Do₁–Do₃ | 8ª baja |
    | **Glockenspiel** | Do₄–Do₆ | Do₆–Do₈ | 15ª alta (2 octavas) |
    | **Xilófono** | Do₃–Do₆ | Do₄–Do₇ | 8ª alta |
    | **Celesta** | Do₃–Do₆ | Do₄–Do₇ | 8ª alta |
    | **Voz tenor (en clave de Sol)** | Do₃–Do₄ | Do₂–Do₃ | 8ª baja |

    La transposición de octava se indica con un pequeño "8" (o "15" para dos octavas) sobre o bajo la clave. En MuseScore, si agregás el instrumento correcto desde el asistente de nueva partitura, la transposición de octava se configura automáticamente.

    ### Instrumentos NO transpositores (tono escrito = tono de concierto)

    Para referencia, estos son los instrumentos que suenan EXACTAMENTE lo que leés en el pentagrama:

    - Piano, órgano, teclados
    - Flauta traversa (y flauta en Do)
    - Oboe
    - Fagot
    - Violín, viola, violonchelo (el cello NO transpone, aunque lee en clave de Fa)
    - Trombón (en Do, aunque existen trombones en Si♭ que son no transpositores porque se leen en Do)
    - Tuba (en Do, aunque hay tubas en Si♭ y Mi♭ que SÍ transponen en bandas británicas de metales)
    - Voz humana (todas las cuerdas)
    - Percusión de altura determinada (marimba, vibráfono, timbales)

???+ note "El caso especial: percusión transpositora"

    Aunque en sesiones anteriores dijimos que la percusión "no transpone" en el sentido tonal, HAY instrumentos de percusión que son transpositores de octava y DEBEN configurarse correctamente en MuseScore.

    | Instrumento | Transposición |
    |---|---|
    | **Glockenspiel** | Suena 2 octavas arriba de lo escrito (15ª alta) |
    | **Xilófono** | Suena 1 octava arriba |
    | **Celesta** | Suena 1 octava arriba |
    | **Campanas tubulares (chimes)** | Suena 1 octava arriba |
    | **Crótalos (antique cymbals)** | Suena 2 octavas arriba |

    Estos instrumentos se escriben en su registro cómodo (evitando líneas adicionales) pero suenan más agudos. En MuseScore, al seleccionar el instrumento correcto, la transposición de octava se aplica automáticamente. Si escribís un Do₄ para glockenspiel, MuseScore lo reproduce como Do₆.

???+ note "Escribir correctamente para instrumentos transpositores: checklist"

    Este es el checklist definitivo para no equivocarte al escribir para una orquesta, banda o ensamble con instrumentos transpositores.

    ### Antes de empezar a escribir

    - [ ] **Decidí la tonalidad de concierto.** ¿En qué tonalidad va a SONAR la obra? Ejemplo: Mi♭ Mayor (3 bemoles).
    - [ ] **Listá los instrumentos y su transposición.** Hacé una tabla rápida: clarinete en Si♭ → +2 ♯, trompa en Fa → +1 ♯, saxofón alto en Mi♭ → +3 ♯, etc.
    - [ ] **Verificá los rangos.** El clarinete en Si♭ no puede tocar un Mi₂ de concierto (su nota más grave es Mi₃ escrito, que suena como Re₃). La trompa tiene un rango de casi 4 octavas pero su registro agudo es muy exigente.

    ### Durante la composición (en tono de concierto)

    - [ ] **Trabajá SIEMPRE en vista de tono de concierto.** Usá el botón de tono de concierto para ver las notas a la altura que suenan. Componé, armonizá y orquestá en esta vista.
    - [ ] **No te preocupes por las armaduras de los instrumentos.** En tono de concierto, todos los pentagramas muestran la MISMA armadura (la de concierto). MuseScore se encarga de transponer las armaduras cuando generes las partes.
    - [ ] **Cuidado con los cruces de registro.** En tono de concierto, un clarinete puede "meterse" visualmente en el registro del fagot. Es normal. Confiá en que cuando imprimas las partes individuales, cada músico verá su parte correctamente.

    ### Al generar las partes (en tono escrito)

    - [ ] **Desactivá el tono de concierto** para ver la partitura general en tono escrito. Verificá que las armaduras de cada instrumento sean las correctas.
    - [ ] **Generá las partes individuales** (Archivo → Partes...). Cada parte DEBE mostrar la armadura correspondiente al instrumento.
    - [ ] **Verificá las partes una por una.** Abrí la parte del clarinete en Si♭. Si la obra está en Mi♭ Mayor concierto, la parte del clarinete debe mostrar 1 bemol (Fa Mayor). Si muestra 3 bemoles, algo está MAL configurado.
    - [ ] **Revisá las notas extremas.** En la parte impresa del clarinete, la nota más grave debe ser Mi₃ (escrito). Si ves un Re₃, está fuera de rango.


---

## Actividad en Classroom

### Tarea: S20 — Transposición y escritura para instrumentos transpositores

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S20_transporte.mscz`, una partitura para piano solo en Sol Mayor (1 sostenido), 4/4, 16 compases, con una melodía diatónica en la mano derecha (Do₄–Sol₅) y acompañamiento de acordes en la mano izquierda; (b) `ejercicio_S20_armadura.mscz`, una partitura para cuarteto de vientos: flauta (no transpone), clarinete en Si♭, trompa en Fa, y fagot (no transpone), en Mi♭ Mayor (3 bemoles), 4/4, 24 compases, con una melodía simple en la flauta y notas largas (redondas y blancas) en los otros instrumentos; (c) `ejercicio_S20_banda.mscz`, una partitura para ensamble de vientos: flauta, clarinete en Si♭, saxofón alto en Mi♭ y saxofón tenor en Si♭, en Fa Mayor (1 bemol), 4/4, 20 compases, con melodía, sin armaduras transpuestas configuradas (todos los pentagramas muestran la misma armadura incorrectamente).

1. **Transposición básica de tonalidad.** Abrí `ejercicio_S20_transporte.mscz`:
    - La pieza está en Sol Mayor (1 sostenido). Transportala a las siguientes tonalidades usando **Herramientas → Transponer → A una tonalidad**.
    - Para CADA nueva tonalidad, guardá una copia del archivo con nombre descriptivo:
      - A La Mayor (3 sostenidos) → `APELLIDO_S20_transporte_LaM.mscz`
      - A Mi♭ Mayor (3 bemoles) → `APELLIDO_S20_transporte_MibM.mscz`
      - A Mi Mayor (4 sostenidos) → `APELLIDO_S20_transporte_MiM.mscz`
    - En cada copia, verificá: (a) que la armadura haya cambiado correctamente, (b) que las alteraciones accidentales se hayan ajustado, (c) que las notas sigan estando en el rango cómodo del piano (verificá que no haya notas fuera del teclado estándar de 88 teclas).
    - Reproducí las cuatro versiones (original + 3 transportadas). ¿La melodía mantiene las mismas relaciones interválicas? (Debería: es la MISMA melodía, solo cambió la altura absoluta.)

2. **Armaduras para instrumentos transpositores.** Abrí `ejercicio_S20_armadura.mscz`:
    - La pieza está en Mi♭ Mayor (3 bemoles) en tono de concierto. Activá el botón **Tono de concierto** para verificar que todos los pentagramas muestren 3 bemoles.
    - Ahora desactivá el **Tono de concierto**. Observá lo que sucede:
      - La flauta (no transpone) debería seguir mostrando Mi♭ Mayor (3 ♭). ¿Es así?
      - El clarinete en Si♭ debería mostrar 1 bemol (Fa Mayor). ¿Es así? Si no, la configuración del instrumento está mal.
      - La trompa en Fa debería mostrar 2 bemoles (Si♭ Mayor). ¿Es así? Si no, configurala.
      - El fagot (no transpone) debería seguir mostrando Mi♭ Mayor (3 ♭). ¿Es así?
    - Para cada instrumento que muestre una armadura incorrecta, corregila desde **Propiedades del pentagrama → Transposición** configurando el intervalo correcto.
    - Alterná varias veces entre tono de concierto y tono escrito (`Ctrl + Shift + C`). Familiarizate con el "baile" de armaduras. Entendé que ninguna nota "cambió": solo cambió lo que VES.
    - Agregá un Staff Text (`Ctrl + T`) en el primer compás de cada instrumento que indique: "Escrito en [tonalidad]" (ej. "Escrito en Fa Mayor" para el clarinete).

3. **Corrección de banda mal configurada.** Abrí `ejercicio_S20_banda.mscz`:
    - Este archivo tiene un ERROR DELIBERADO: todos los pentagramas muestran la misma armadura (Fa Mayor, 1 bemol), incluso los instrumentos transpositores. Esto es INCORRECTO.
    - Activá el tono de concierto. ¿Qué tonalidad muestra? Debería ser Fa Mayor para todos.
    - Desactivá el tono de concierto. Ahora verificá cada instrumento:
      - **Clarinete en Si♭**: debería mostrar Sol Mayor (1 ♯). Corregilo en Propiedades del pentagrama.
      - **Saxofón alto en Mi♭**: debería mostrar Re Mayor (2 ♯). Corregilo.
      - **Saxofón tenor en Si♭**: debería mostrar Sol Mayor (1 ♯). Corregilo.
    - Después de corregir, alterná entre tono de concierto y tono escrito para confirmar que todo funciona.
    - Generá las partes individuales para cada instrumento: **Archivo → Partes → Generar**. Verificá que cada parte tenga la armadura CORRECTA para ese instrumento.
    - Exportá las 4 partes como PDF (una por instrumento).

4. **Transposición de orquestación: de piano a cuarteto.** Creá una NUEVA partitura desde cero: `APELLIDO_Nombre_S20_cuarteto.mscz`.
    - Plantilla: seleccioná 4 instrumentos: **Flauta**, **Clarinete en Si♭**, **Violín** (no transpone) y **Violonchelo** (no transpone, en clave de Fa).
    - Tonalidad de concierto: Re Mayor (2 sostenidos). Compás: 3/4.
    - **Melodía**: en los primeros 8 compases, escribí una melodía para flauta en Re Mayor. Usá negras, corcheas y alguna blanca.
    - **Transposición al clarinete**: copiá la melodía de la flauta (compases 1–8) al clarinete, pero transportada: el clarinete en Si♭ debe leer un tono por ENCIMA para sonar igual que la flauta. Hacelo así:
      - Seleccioná la melodía de la flauta.
      - Copiala al pentagrama del clarinete.
      - Con el tono de concierto DESACTIVADO, seleccioná todo el pentagrama del clarinete y usá **Herramientas → Transponer → Por intervalo → 2ª mayor ascendente**.
      - Ahora el clarinete lee un tono arriba de lo que lee la flauta, pero SUENA IGUAL. Verificá activando el tono de concierto.
    - **Armonía**: escribí una línea de violín (contramelodía en corcheas) y una línea de violonchelo (bajo en redondas y blancas) que acompañen la melodía en Re Mayor.
    - Reproducí. La flauta y el clarinete deben sonar AL UNÍSONO (o en octavas si el rango lo requiere) durante los compases 1–8.
    - Exportá como PDF con el tono escrito DESACTIVADO (para que los músicos vean lo que deben leer).

5. **Integración: partitura para banda de vientos.** Creá una NUEVA partitura: `APELLIDO_Nombre_S20_banda.mscz`.
    - Plantilla: **Flauta**, **Clarinete en Si♭**, **Saxofón alto en Mi♭**, **Saxofón tenor en Si♭**, **Trompeta en Si♭**, **Trombón** (no transpone, clave de Fa).
    - Tonalidad de concierto: Si♭ Mayor (2 bemoles). Compás: 4/4. 24 compases.
    - **Componé en tono de concierto.** Creá una pieza corta con:
      - **Flauta + Clarinete**: melodía principal (al unísono o en octavas).
      - **Saxofón alto + Saxofón tenor**: contramelodía o armonía en bloque.
      - **Trompeta**: melodía secundaria (contesta a la flauta/clarinete en frases alternadas).
      - **Trombón**: línea de bajo.
    - **Verificá las armaduras en tono escrito.** Desactivá el tono de concierto. Cada instrumento debe mostrar su armadura correcta:
      - Flauta: Si♭ Mayor (2 ♭)
      - Clarinete en Si♭: Do Mayor (0 alteraciones)
      - Saxofón alto en Mi♭: Sol Mayor (1 ♯)
      - Saxofón tenor en Si♭: Do Mayor (0 alteraciones)
      - Trompeta en Si♭: Do Mayor (0 alteraciones)
      - Trombón: Si♭ Mayor (2 ♭)
    - **Generá las partes individuales** y exportá el PDF de cada parte.
    - **Generá la partitura general** (full score) en tono escrito y exportala como PDF.

6. **Reflexión sobre transposición.** En Classroom, respondé:
    - Explicá con tus propias palabras por qué existen los instrumentos transpositores. No repitas lo que dice el glosario: explicá el concepto como si se lo estuvieras contando a un compañero que no entiende nada del tema.
    - Si estuvieras componiendo para una orquesta sinfónica, ¿en qué vista trabajarías (tono de concierto o tono escrito) y por qué? ¿En qué momento cambiarías de vista?
    - Un clarinetista te dice: "Tu partitura está mal, dijiste que era en Mi♭ Mayor pero mi parte tiene un bemol." ¿Está en lo correcto el clarinetista? ¿Por qué? Explicá qué está pasando realmente.

### Entregables

- [ ] `APELLIDO_S20_transporte_LaM.mscz` y `.pdf`
- [ ] `APELLIDO_S20_transporte_MibM.mscz` y `.pdf`
- [ ] `APELLIDO_S20_transporte_MiM.mscz` y `.pdf`
- [ ] `APELLIDO_S20_armadura_corregida.mscz` (cuarteto con armaduras corregidas + Staff Texts)
- [ ] `APELLIDO_S20_armadura_corregida.pdf`
- [ ] `APELLIDO_S20_banda_corregida.mscz` + PDFs de las 4 partes individuales (flauta, clarinete, saxofón alto, saxofón tenor)
- [ ] `APELLIDO_Nombre_S20_cuarteto.mscz` y `.pdf`
- [ ] `APELLIDO_Nombre_S20_banda.mscz` + PDF de la partitura general + PDFs de las 6 partes individuales
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) breve explicación de qué fue lo más difícil de entender sobre la transposición y cómo lo resolviste.

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Transposición de tonalidad | 3 transposiciones correctas; notas en rango; armaduras bien aplicadas | 2 correctas o con errores menores de rango | ≤1 correcta |
| Armaduras transpositoras | Armaduras corregidas para clarinete (Si♭→Fa Mayor) y trompa (Fa→Si♭ Mayor); Staff Texts de identificación presentes | Una armadura correcta, otra incorrecta | Ninguna armadura corregida |
| Banda mal configurada | Clar, sax alto, sax tenor con armaduras corregidas; partes individuales generadas y exportadas correctamente | 2 de 3 instrumentos corregidos | ≤1 instrumento corregido |
| Cuarteto flauta/clarinete/violín/cello | Melodía compartida Fl+Cl al unísono (con transporte correcto); contramelodía y bajo en Re Mayor; armaduras correctas | Errores en transporte del clarinete (no suena al unísono) o armaduras incorrectas | Clar transporte incorrecto; no suena como la flauta |
| Partitura para banda | 6 instrumentos; composición en Si♭ Mayor; todas las armaduras correctas en tono escrito; partes y full score exportados | 4–5 instrumentos bien configurados o faltan partes | ≤3 instrumentos bien configurados |
| Reflexión | 3 respuestas correctas y con comprensión conceptual del porqué de la transposición | 2 respuestas correctas | ≤1 respuesta correcta |

---

*Basado en: MuseScore Studio 4 Handbook — Notation: Transposition, Concert pitch, Sound and playback | https://handbook.musescore.org*
