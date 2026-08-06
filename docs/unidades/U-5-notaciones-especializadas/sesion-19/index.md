# Sesión 19: Tablatura y notación para guitarra

📚 Handbook → Notation: Tablature | Advanced topics: Fretboard diagrams | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="tablatura"></a> **Tablatura (tablature / TAB)** | Sistema de notación para instrumentos de cuerda con trastes (guitarra, bajo, ukelele, laúd) donde cada línea horizontal representa una cuerda del instrumento y los números sobre las líneas indican el traste que debe pisarse. La línea superior corresponde a la primera cuerda (la más aguda) y la inferior a la sexta (la más grave). |
    | <a id="traste"></a> **Traste (fret)** | Barra metálica incrustada en el diapasón de la guitarra que divide las cuerdas en semitonos. El número en una tablatura indica qué traste pisar: 0 = cuerda al aire, 1 = primer traste, 2 = segundo, etc. Cada traste equivale a un semitono ascendente desde la cuerda al aire. |
    | <a id="cuerda"></a> **Cuerda (string)** | En la guitarra estándar, las 6 cuerdas se afinan (de aguda a grave): Mi₄ (1ª), Si₃ (2ª), Sol₃ (3ª), Re₃ (4ª), La₂ (5ª), Mi₂ (6ª). En la tablatura, se representan como 6 líneas horizontales: la 1ª cuerda arriba, la 6ª abajo. El bajo eléctrico estándar tiene 4 cuerdas: Sol₂, Re₂, La₁, Mi₁. |
    | <a id="bend"></a> **Bend / Estiramiento** | Técnica donde el guitarrista empuja o jala la cuerda hacia arriba/abajo para elevar la afinación de la nota de forma gradual. Se indica con una flecha curva hacia arriba y la cantidad de tonos que se eleva: *full* (1 tono), *1/2* (medio tono), *1 1/2* (tono y medio). En MuseScore, se inserta como una línea de bend desde la paleta **Líneas** o como una articulación. |
    | <a id="slide"></a> **Slide / Deslizamiento / Glissando** | Técnica donde el dedo se desliza sobre la cuerda de un traste a otro sin levantar la presión, produciendo un barrido continuo de altura. Puede ser ascendente (slide up) o descendente (slide down). Se indica con una línea inclinada entre dos notas. En MuseScore, se inserta desde la paleta **Líneas → Glissando** o con la articulación de slide. |
    | <a id="hammer-on"></a> **Hammer-on / Ligado ascendente** | Técnica donde una nota se produce golpeando la cuerda con un dedo de la mano izquierda sin pulsarla de nuevo con la derecha. Es decir, la primera nota se pulsa normalmente y la segunda "suena sola" por el golpe del dedo. Se indica con un arco (ligadura) entre las dos notas. En notación de guitarra, el arco con una "H" sobre él confirma que es hammer-on. |
    | <a id="pull-off"></a> **Pull-off / Ligado descendente** | Técnica opuesta al hammer-on: un dedo de la mano izquierda se retira de la cuerda "pellizcándola" para que suene la nota inferior sin pulsar de nuevo. También se indica con un arco entre las notas, a veces con una "P" sobre él. |
    | <a id="vibrato"></a> **Vibrato de guitarra** | Oscilación de la altura de una nota producida moviendo el dedo hacia arriba y abajo sobre el traste (vibrato de mano izquierda) o usando la palanca de trémolo. Se indica con una línea ondulada sobre la nota. En MuseScore, se inserta desde la paleta **Líneas → Vibrato**. |
    | <a id="palm-mute"></a> **Palm mute / Apagado con palma** | Técnica donde la palma de la mano derecha se apoya suavemente sobre las cuerdas cerca del puente, produciendo un sonido apagado y percusivo. Se indica con "P.M." o "palm mute" sobre las notas afectadas, a menudo con una línea punteada que marca la duración del efecto. |
    | <a id="armonico"></a> **Armónico (harmonic)** | Sonido producido al rozar la cuerda en puntos nodales específicos (trastes 5, 7, 12, etc.) en lugar de pisarla completamente. Los armónicos naturales suenan como campanas. En tablatura, se indican con el número del traste entre paréntesis angulares `<7>`, `<12>` o con la abreviatura "harm." En notación estándar, la cabeza de la nota es un diamante (rombo). |
    | <a id="diagrama-trastero"></a> **Diagrama de trastes (fretboard diagram)** | Representación visual del diapasón de la guitarra que muestra la posición de los dedos para formar un acorde. Las líneas verticales son las cuerdas, las horizontales son los trastes. Puntos negros indican dónde pisar, círculos blancos indican cuerdas al aire, y X indica cuerdas que no se tocan. MuseScore los genera automáticamente a partir del cifrado armónico. |
    | <a id="afinacion-alterna"></a> **Afinación alternativa (alternate tuning)** | Cuando la guitarra se afina diferente al estándar Mi-Si-Sol-Re-La-Mi. Ejemplos: Drop D (6ª cuerda baja a Re), Open G (Sol-Re-Sol-Si-Re-Sol para slide con bottleneck), DADGAD (música celta/folk). La tablatura refleja la afinación escribiendo el nombre de cada cuerda al inicio del pentagrama. |

???+ note "Tablatura: el mapa directo del diapasón"

    La tablatura (TAB) es el sistema de notación más antiguo para instrumentos de cuerda, anterior al pentagrama tradicional. Hoy convive con la notación estándar como un complemento indispensable para guitarristas.

    ### Anatomía de una tablatura

    ```
    Guitarra estándar (afinación EADGBE):
    
    e ||--0---1---3---1---0----|  ← 1ª cuerda (Mi₄, la más aguda)
    B ||--1---3---3---1---1----|  ← 2ª cuerda (Si₃)
    G ||--0---2---2---2---0----|  ← 3ª cuerda (Sol₃)
    D ||--2---0---0---3---2----|  ← 4ª cuerda (Re₃)
    A ||--3-------------------|  ← 5ª cuerda (La₂)
    E ||----------------------|  ← 6ª cuerda (Mi₂, la más grave)
    ```

    Reglas fundamentales:
    1. **Las líneas son cuerdas, no notas.** La línea superior = 1ª cuerda (más aguda). La línea inferior = 6ª cuerda (más grave). Esto es AL REVÉS de la intuición visual (normalmente "arriba" es grave), pero tiene lógica: cuando mirás la guitarra desde arriba, la 1ª cuerda está más cerca de tu cara.
    2. **Los números son trastes, no duraciones.** 0 = cuerda al aire, 1 = primer traste, 3 = tercer traste, etc. La duración (negra, corchea) se indica con las plicas y figuras rítmicas normales que acompañan a los números.
    3. **Las cuerdas se nombran al inicio.** La afinación estándar se escribe a la izquierda del pentagrama TAB: `e`, `B`, `G`, `D`, `A`, `E` (de aguda a grave). Para afinaciones alternativas, se escriben las notas correspondientes.

    ### Tablatura vs. pentagrama estándar

    | Característica | Pentagrama estándar | Tablatura |
    |---|---|---|
    | **Qué muestra** | La altura de la nota (Do, Re, Mi) | DÓNDE tocar la nota (cuerda + traste) |
    | **Curva de aprendizaje** | Alta (requiere leer música) | Baja (intuitiva para guitarristas) |
    | **Información rítmica** | Completa (figuras y silencios) | Depende: las tablaturas profesionales incluyen plicas y figuras; las tablaturas amateur, no. |
    | **Digitación** | Implícita (la misma nota puede tocarse en varias posiciones) | Explícita (muestra exactamente qué traste y cuerda) |
    | **Transporte** | Fácil (cambiar armadura) | Imposible (cada afinación requiere tablatura nueva) |

    !!! tip "La tablatura NO reemplaza al pentagrama"
        La tablatura te dice DÓNDE poner los dedos. El pentagrama te dice QUÉ sonido producir. Un músico completo necesita AMBOS: la tablatura para aprender rápido una canción, el pentagrama para entender la música. En MuseScore, la forma profesional es MOSTRAR AMBOS SIMULTÁNEAMENTE: pentagrama estándar arriba y tablatura abajo, vinculados como un solo instrumento.

    ### Crear una tablatura en MuseScore

    1. Crear nueva partitura → **Cuerdas → Guitarra → Guitarra + Tablatura** (o **Bajo + Tablatura**).
    2. MuseScore crea automáticamente un sistema de DOS pentagramas vinculados: el pentagrama estándar arriba y la tablatura abajo.
    3. Ingresar las notas en el pentagrama estándar normalmente. MuseScore las refleja automáticamente en la tablatura, eligiendo la posición (cuerda/traste) más lógica.
    4. Si MuseScore elige una posición que no es la que querés (ej. tocar un Mi₄ en la 2ª cuerda traste 5 en lugar de 1ª cuerda al aire), seleccioná la nota en la tablatura y movela con `Ctrl + ↑ / ↓` para cambiar de cuerda.

    > Insertar captura de un sistema guitarra + tablatura en MuseScore mostrando el pentagrama estándar arriba y la tablatura abajo, con una melodía simple (escala de Do mayor en primera posición) reflejada en ambos.

???+ note "Técnicas de guitarra en notación: bends, slides, hammer-ons y más"

    La guitarra eléctrica, en particular, tiene un vocabulario técnico extenso que el compositor debe poder comunicar con precisión.

    ### Bend (estiramiento)

    El bend es el "efecto vocal" de la guitarra: la nota llora, se desliza microtonalmente hacia arriba.

    | Tipo de bend | Indicación visual | Significado |
    |---|---|---|
    | **Bend de un tono (full)** | Flecha curva con "full" | Estirar hasta que la nota suene un tono entero más agudo |
    | **Bend de medio tono (1/2)** | Flecha curva con "1/2" | Estirar medio tono |
    | **Bend y release** | Flecha sube y luego baja | Estirar y luego volver a la nota original |
    | **Pre-bend** | Flecha que empieza ya arriba | La cuerda ya está estirada ANTES de pulsarla; luego se libera |
    | **Bend progresivo** | Flecha curva larga | Estiramiento lento y gradual |

    **Cómo insertar un bend en MuseScore:**

    1. Seleccionar la nota de origen.
    2. Ir a la paleta **Líneas** → buscar **Bend** (o **Guitar bend**).
    3. Arrastrar el bend sobre la nota.
    4. Ajustar la cantidad (full, 1/2, 1 1/2) desde el panel **Propiedades** o haciendo clic derecho en el bend → **Propiedades del bend**.

    !!! warning "El bend en la tablatura"
        En la tablatura, un bend se ve así:
        ```
        e ||--7b9----|   (traste 7 estirado hasta sonar como traste 9 = bend de un tono)
        ```
        El número antes de la "b" es el traste pisado. El número después es el traste equivalente al sonido resultante. MuseScore genera esta notación automáticamente cuando insertás un bend en el pentagrama estándar.

    ### Slide (deslizamiento)

    | Tipo de slide | Indicación | Significado |
    |---|---|---|
    | **Slide ascendente (slide up)** | Línea inclinada hacia arriba | Deslizar el dedo hacia trastes más agudos |
    | **Slide descendente (slide down)** | Línea inclinada hacia abajo | Deslizar hacia trastes más graves |
    | **Slide de entrada (slide in)** | Línea desde abajo hacia la nota | Empezar el slide desde un traste indefinido y llegar a la nota |
    | **Slide de salida (slide out)** | Línea desde la nota hacia abajo | Deslizar hacia un traste indefinido después de tocar |

    **Cómo insertar un slide en MuseScore:**

    1. Seleccionar la nota de origen.
    2. Ir a la paleta **Líneas → Glissando** (mismo símbolo que para arpa o trombón) o buscar **Slide** en la paleta de articulaciones de guitarra.
    3. Arrastrar el símbolo sobre la nota.
    4. Si el slide es entre dos notas concretas, seleccionar ambas notas y aplicar el glissando entre ellas.

    > Insertar captura de un pasaje de guitarra con: bend de un tono (7b9), slide ascendente (5/7), hammer-on (5h7) y pull-off (7p5), todo en contexto de un lick de blues.

    ### Hammer-on y Pull-off (ligados de guitarra)

    En notación de guitarra, el arco de ligadura tiene un significado diferente al de otros instrumentos:

    | Técnica | Notación | Significado |
    |---|---|---|
    | **Hammer-on** | Arco entre dos notas, con "H" encima | Tocar la primera nota normalmente, producir la segunda golpeando la cuerda con un dedo de la mano izquierda |
    | **Pull-off** | Arco entre dos notas, con "P" encima | Tocar la primera nota, retirar el dedo "pellizcando" la cuerda para que suene la segunda |
    | **Tap (tapping)** | Arco con "T" encima | Producir la nota golpeando la cuerda con un dedo de la mano DERECHA sobre el diapasón (técnica de guitarra eléctrica moderna) |

    **Cómo insertar en MuseScore:**

    1. Seleccionar las dos notas.
    2. Agregar una ligadura normal (`S` o desde la paleta **Líneas → Slur**). MuseScore la dibuja como un arco.
    3. Agregar la letra "H", "P" o "T" como Staff Text (`Ctrl + T`) sobre la ligadura para especificar la técnica.
    4. En la tablatura, el hammer-on se ve como un arco entre dos números; el pull-off, igual. La letra H o P ayuda a distinguirlos.

    ### Vibrato y palm mute

    - **Vibrato**: Paleta **Líneas → Vibrato**. Arrastrar sobre la nota. Se puede ajustar la longitud y la intensidad.
    - **Palm mute**: Escribir "P.M." como Staff Text al inicio del pasaje, y agregar una línea punteada (paleta **Líneas**) que se extienda hasta donde termina el efecto. Las notas bajo palm mute se escriben normalmente.

    ### Armónicos

    - **Armónico natural**: cabeza de nota en forma de diamante (rombo) y la indicación "harm." o "nat. harm." como Staff Text.
    - **Armónico artificial**: cabeza de diamante con la indicación "A.H." (artificial harmonic). En tablatura, el número del traste entre paréntesis angulares: `<7>`, `<12>`.
    - En MuseScore: seleccionar la nota → Paleta **Cabezas de nota → Diamante** + Staff Text "harm."

???+ note "Diagramas de trastes: el acorde en una imagen"

    Los diagramas de trastes (fretboard diagrams) son la representación visual de un acorde en el diapasón. Son omnipresentes en cancioneros, *fake books* y partituras de guitarra.

    ### Lectura de un diagrama de trastes

    ```
         C (Do mayor)
    e ||--0--------  ← cuerda al aire (círculo blanco)
    B ||--1--------  ← traste 1, dedo 1 (índice)
    G ||--0--------  ← cuerda al aire
    D ||--2--------  ← traste 2, dedo 2 (medio)
    A ||--3--------  ← traste 3, dedo 3 (anular)
    E ||--X--------  ← cuerda no se toca (X)
         |  |  |
         1º 2º 3º traste
    ```

    Elementos del diagrama:
    - **Líneas verticales**: cuerdas (izquierda = 6ª Mi grave, derecha = 1ª Mi aguda).
    - **Líneas horizontales**: trastes (la línea superior gruesa es la cejilla/cejuela; debajo, trastes 1, 2, 3...).
    - **Punto negro**: cuerda pisada en ese traste. A veces el número dentro del punto indica qué dedo usar (1=índice, 2=medio, 3=anular, 4=meñique).
    - **Círculo blanco (O)**: cuerda al aire (se toca sin pisar).
    - **X**: cuerda que NO se toca (se apaga o se omite).
    - **Barra / cejilla**: línea gruesa horizontal que cruza varias cuerdas → un solo dedo (generalmente el índice) pisa todas esas cuerdas a la vez.

    ### Generar diagramas de trastes en MuseScore

    MuseScore puede generar automáticamente diagramas de trastes a partir del cifrado armónico:

    1. Asegurate de tener un pentagrama de guitarra vinculado a una tablatura (o al menos un pentagrama de guitarra en la partitura).
    2. Ingresá el cifrado armónico normalmente (`Ctrl + K`): `C`, `Am`, `G7`, `Dm7`, etc.
    3. Seleccioná la primera nota con cifrado.
    4. Andá a **Añadir → Texto → Diagrama de trastes** (o usá la paleta **Diagramas de trastes**).
    5. MuseScore genera automáticamente un diagrama para ese acorde. Si hay múltiples posiciones posibles (ej. Do mayor puede tocarse en posición abierta o con cejilla en el traste 8), MuseScore elige una por defecto.
    6. Para cambiar la posición del diagrama: seleccionalo → panel **Propiedades → Diagrama de trastes** → elegir otra posición o editar manualmente.

    !!! tip "Diagramas vs. cifrado vs. tablatura: ¿cuál uso?"
        - **Diagrama de trastes**: para cancioneros y *lead sheets* de guitarra. El guitarrista ve el acorde y lo toca. Ideal para acompañamiento.
        - **Cifrado americano**: para cualquier instrumento armónico (piano, guitarra, acordeón). Es universal.
        - **Tablatura**: para melodías y solos donde la digitación exacta es crítica. Ideal para aprender una canción nota por nota.
        - **Los tres juntos**: la forma más completa de escribir para guitarra en MuseScore: pentagrama estándar + tablatura + cifrado americano + diagramas de trastes. El guitarrista elige qué capa de información usar.

    > Insertar captura de un sistema de guitarra en MuseScore con: pentagrama estándar (melodía con plicas), tablatura (número de trastes), cifrado americano (C, Am, G7), y diagramas de trastes sobre el primer acorde de cada cambio.

???+ note "Afinaciones alternativas y bajo eléctrico"

    La notación de guitarra se complica cuando el instrumento no está en afinación estándar.

    ### Afinaciones alternativas comunes

    | Afinación | Cuerdas (de aguda a grave) | Se usa en... | Particularidad |
    |---|---|---|---|
    | **Estándar** | E B G D A E | Todo | La referencia universal |
    | **Drop D** | E B G D A **D** | Rock, metal, grunge | Solo baja la 6ª cuerda un tono. Acordes de potencia (power chords) con un solo dedo. |
    | **Open G** | D B G D **G** **D** | Blues con slide (bottleneck), Rolling Stones | Afinación que produce un acorde de Sol mayor al tocar todas las cuerdas al aire. |
    | **Open D** | D A F♯ D A D | Blues, folk con slide | Acorde de Re mayor al aire. Muy usado para slide. |
    | **DADGAD** | D A G D **A** D | Música celta, folk, fingerstyle | Sonoridad modal y abierta. Popularizado por guitarristas folk británicos. |
    | **Half-step down (Eb)** | E♭ B♭ G♭ D♭ A♭ E♭ | Rock, metal (Jimi Hendrix, Slayer) | Todas las cuerdas medio tono abajo. Sonido más oscuro, cuerdas más sueltas. |
    | **Bajo estándar** | G D A E | Todo para bajo eléctrico | Mismas notas que las 4 cuerdas graves de la guitarra pero una octava abajo. |

    ### Cómo configurar afinaciones alternativas en MuseScore

    1. Seleccionar el pentagrama de guitarra/bajo.
    2. Ir a **Propiedades del pentagrama** (clic derecho en el pentagrama → **Propiedades del pentagrama/parte**).
    3. En la sección **Cuerdas**, editar la afinación de cada cuerda. Se puede cambiar la nota y la octava.
    4. MuseScore ajusta automáticamente la tablatura y la notación estándar para reflejar la nueva afinación.

    !!! warning "Cuidado con las notas fuera de rango"
        Si bajás una cuerda más de un tono (ej. Drop C: 6ª cuerda baja a Do₂), algunas notas pueden quedar fuera del rango reproducible o visualmente extrañas en el pentagrama estándar. Verificá que las notas sigan siendo legibles.

    ### Bajo eléctrico

    El bajo se escribe en clave de Fa, una octava arriba de su sonido real (es un instrumento transpositor: suena una octava más grave de lo escrito). La tablatura de bajo usa 4 líneas (4 cuerdas) en lugar de 6:

    ```
    Bajo estándar (afinación EADG):
    
    G ||-------------------|  ← 1ª cuerda (Sol₂, la más aguda)
    D ||-------------------|  ← 2ª cuerda (Re₂)
    A ||-------------------|  ← 3ª cuerda (La₁)
    E ||--3---5---5---3----|  ← 4ª cuerda (Mi₁, la más grave)
    ```

    Las técnicas de bajo son similares a la guitarra pero con énfasis en slides, hammer-ons/pull-offs y, sobre todo, SLAP (golpe con el pulgar) y POP (tirar de la cuerda con el índice), que se indican con "S" y "P" como Staff Text sobre las notas afectadas.

---

## Actividad en Classroom

### Tarea: S19 — Tablatura y notación para guitarra

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S19_tab.mscz`, una partitura de guitarra con pentagrama estándar + tablatura vinculados, en Mi menor, 4/4, 16 compases, con una melodía en el pentagrama estándar que debe ser verificada y corregida en la tablatura (algunas notas están en posiciones ineficientes); (b) `ejercicio_S19_tecnicas.mscz`, una partitura para guitarra eléctrica (pentagrama estándar + tablatura) en La menor pentatónica, 4/4, 20 compases, con una melodía escrita pero SIN indicaciones de bends, slides, hammer-ons, pull-offs ni vibrato (solo las notas "peladas"); (c) `ejercicio_S19_diagramas.mscz`, una partitura para guitarra en Sol mayor, 4/4, 24 compases con una melodía y cifrado armónico ya ingresado (`G`, `C`, `D`, `Em`, `Am`, `Bm`) pero SIN diagramas de trastes.

1. **Tablatura: verificá las posiciones.** Abrí `ejercicio_S19_tab.mscz`:
    - Reproducí la melodía para familiarizarte con ella.
    - Mirá la tablatura generada automáticamente por MuseScore. Identificá al menos 5 notas donde la posición elegida por MuseScore NO es la más eficiente para un guitarrista (por ejemplo: tocar un Mi₄ en la 2ª cuerda traste 5 cuando podría ser 1ª cuerda al aire; o saltos innecesarios de la 1ª a la 4ª cuerda).
    - Para cada nota ineficiente, seleccionala en la tablatura y movela a la cuerda/traste correcto usando `Ctrl + ↑ / ↓` (dentro del pentagrama de tablatura). Verificá que la nota en el pentagrama estándar NO cambie (debe seguir sonando igual).
    - Agregá un breve comentario como Staff Text (`Ctrl + T`) en la primera ocurrencia de cada corrección explicando por qué la nueva posición es mejor: "mejor en 1ª al aire que 2ª traste 5", "evitar salto de 4ª a 1ª cuerda", etc.
    - Reproducí de nuevo: ¿la melodía suena igual pero es más fácil de tocar?

2. **Técnicas de guitarra: dale vida al solo.** Abrí `ejercicio_S19_tecnicas.mscz`:
    - Escuchá la melodía. Es un solo de guitarra en La menor pentatónica pero sin expresión: todas las notas están "planas", sin bends ni slides.
    - **Bends**: identificá al menos 4 lugares donde un bend mejoraría la expresión. Insertá bends de los siguientes tipos (paleta **Líneas → Bend**):
      - 2 bends de un tono (full) en notas largas (blancas o redondas).
      - 1 bend de medio tono (1/2).
      - 1 bend con release (sube y vuelve a bajar).
    - **Slides**: insertá al menos 3 slides (paleta **Líneas → Glissando**):
      - 2 slides ascendentes entre notas diferentes.
      - 1 slide descendente.
    - **Hammer-ons y Pull-offs**: insertá al menos 4 ligaduras de guitarra (arco `S` + Staff Text "H" o "P" encima):
      - 2 hammer-ons (nota grave → aguda).
      - 2 pull-offs (nota aguda → grave).
    - **Vibrato**: agregá vibrato (paleta **Líneas → Vibrato**) en al menos 2 notas sostenidas al final de frases.
    - Reproducí el solo con todas las técnicas. ¿Ahora suena como un solo de guitarra real? ¿Los bends se escuchan? ¿Los slides y hammer-ons cambian la articulación?

3. **Diagramas de trastes: la chuleta visual.** Abrí `ejercicio_S19_diagramas.mscz`:
    - El archivo ya tiene cifrado armónico (`G`, `C`, `D`, `Em`, `Am`, `Bm`) sobre la melodía.
    - Seleccioná la primera nota de cada cambio de acorde.
    - Insertá un **diagrama de trastes** para cada acorde: **Añadir → Texto → Diagrama de trastes**, o desde la paleta **Diagramas de trastes**.
    - Verificá que los diagramas sean correctos y estén en posiciones "abiertas" (sin cejilla, trastes bajos) cuando sea posible. Si MuseScore genera un diagrama con cejilla para un acorde que claramente puede tocarse abierto (ej. C, G, D, Em, Am), editá el diagrama desde el panel **Propiedades** y seleccioná la posición abierta.
    - Asegurate de que los diagramas NO se superpongan entre sí ni con el cifrado. Movelos verticalmente si es necesario (arrastrando con el mouse).
    - Exportá como PDF. ¿Los diagramas de trastes son claros y legibles? ¿Un guitarrista podría tocar la canción solo con los diagramas?

4. **Afinaciones alternativas y bajo.** En el mismo archivo `ejercicio_S19_tab.mscz` ya editado:
    - Creá una copia del pentagrama de guitarra. Andá a **Añadir → Instrumentos → Guitarra → Guitarra + Tablatura** para agregar una SEGUNDA guitarra.
    - En esta segunda guitarra, cambiá la afinación a **Drop D** (editá las cuerdas desde Propiedades del pentagrama: bajá la 6ª cuerda de Mi₂ a Re₂).
    - Copiá los primeros 8 compases de la melodía original a esta segunda guitarra. Observá cómo cambia la tablatura: las notas que antes estaban en la 6ª cuerda ahora requieren trastes diferentes (o ya no son posibles en ciertas posiciones).
    - Ajustá las posiciones en la tablatura de Drop D para que la melodía sea tocable (algunas notas que antes estaban en la 6ª cuerda al aire ahora necesitan traste 2; ajustes similares).
    - Agregá un pentagrama de **Bajo eléctrico + Tablatura** (4 cuerdas, afinación estándar EADG).
    - Escribí una línea de bajo simple (redondas y blancas) que siga los cambios de armonía de la melodía. Usá la tablatura de bajo para elegir posiciones cómodas.
    - Reproducí todo junto. ¿Las dos guitarras (estándar y Drop D) suenan igual a pesar de tener tablaturas diferentes? (Deberían, porque la melodía es la misma.)

5. **Integración: lead sheet de guitarra profesional.** Creá una NUEVA partitura desde cero: `APELLIDO_Nombre_S19_guitarra.mscz`.
    - Plantilla: **Guitarra + Tablatura** (pentagrama estándar + tablatura vinculados).
    - Tonalidad: Mi menor (1 sostenido: Fa♯). Compás: 4/4. 32 compases.
    - **Melodía**: Componé una melodía original en Mi menor (podés usar la escala pentatónica de Mi menor: Mi-Sol-La-Si-Re). Usá negras, corcheas y alguna blanca al final de frases.
    - **Técnicas obligatorias**: la melodía DEBE incluir al menos:
      - 3 bends (de diferentes tipos: full, 1/2, release).
      - 3 slides (ascendentes y descendentes).
      - 4 hammer-ons / pull-offs (combinados).
      - 2 vibratos en notas finales de frase.
      - 1 armónico natural (cabeza de diamante + "harm.") en el traste 12 de alguna cuerda.
    - **Cifrado armónico**: ingresá el cifrado (`Ctrl + K`) de una progresión en Mi menor. Progresión sugerida: Em → Am → D → G → C → Am → B7 → Em. Repetila o varíala para cubrir los 32 compases.
    - **Diagramas de trastes**: insertá diagramas de trastes para CADA acorde del cifrado. Verificá que estén en posiciones abiertas o cómodas. Al menos 3 diagramas deben ser diferentes entre sí.
    - **Estilo visual**: la partitura debe verse como una *lead sheet* de guitarra profesional: pentagrama estándar + tablatura + cifrado + diagramas de trastes + técnicas. Todo legible y bien distribuido.
    - Exportá como PDF.

6. **Reflexión sobre notación de guitarra.** En Classroom, respondé:
    - ¿Qué información proporciona la tablatura que el pentagrama estándar NO puede dar? ¿Y al revés? Da ejemplos concretos de cuándo preferirías usar cada una.
    - ¿Por qué creés que la guitarra tiene un sistema de notación "paralelo" (tablatura) que otros instrumentos (piano, violín, flauta) no tienen? ¿Es una ventaja o una limitación?
    - Si tuvieras que escribir una canción para un guitarrista que NO sabe leer tablatura NI pentagrama, ¿cómo le comunicarías lo que tiene que tocar? ¿Qué otros sistemas de notación/proxies existen (YouTube, tutoriales, etc.) y qué limitaciones tienen comparados con la partitura?

### Entregables

- [ ] `APELLIDO_Nombre_S19_tab_v01.mscz` (tablatura corregida + guitarra Drop D + bajo)
- [ ] `APELLIDO_Nombre_S19_tab_v01.pdf`
- [ ] `APELLIDO_Nombre_S19_tecnicas_v01.mscz` (solo con técnicas de guitarra)
- [ ] `APELLIDO_Nombre_S19_tecnicas_v01.pdf`
- [ ] `APELLIDO_Nombre_S19_diagramas_v01.mscz` (diagramas de trastes insertados)
- [ ] `APELLIDO_Nombre_S19_diagramas_v01.pdf`
- [ ] `APELLIDO_Nombre_S19_guitarra_v01.mscz` (lead sheet de guitarra profesional completa)
- [ ] `APELLIDO_Nombre_S19_guitarra_v01.pdf`
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) la progresión de acordes que usaste en tu lead sheet (escribila como secuencia de cifrados), (c) una breve explicación de cómo elegiste las posiciones de los diagramas de trastes (¿por qué abiertos y no con cejilla?)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Corrección de tablatura | ≥5 notas reposicionadas correctamente; justificación clara de cada cambio; la melodía suena igual | 3–4 cambios correctos o justificación incompleta | ≤2 cambios o tablatura empeorada |
| Técnicas de guitarra | ≥4 bends (tipos variados), ≥3 slides, ≥4 hammer-ons/pull-offs, ≥2 vibratos; todos correctamente insertados y audibles | Técnicas presentes pero con 2–3 errores de inserción o audibilidad | ≤4 técnicas totales o mal insertadas |
| Diagramas de trastes | Diagramas para TODOS los acordes del cifrado; posiciones correctas (abiertas donde corresponde); sin superposiciones | Diagramas presentes pero con 2–3 errores de posición o superposición | Faltan diagramas o >3 errores |
| Afinaciones y bajo | Drop D correctamente configurado; tablatura ajustada; bajo con línea coherente y tablatura | Drop D o bajo configurados pero con errores de ajuste | Drop D o bajo no funcionales |
| Lead sheet de guitarra | Melodía original; todas las técnicas obligatorias presentes; cifrado completo; diagramas para todos los acordes; armónico natural incluido | Lead sheet completa pero falta algún elemento obligatorio | Lead sheet incompleta o sin técnicas |
| Reflexión | Responde las 3 preguntas con profundidad; demuestra comprender las ventajas y limitaciones de cada sistema de notación | Responde 2 de 3 correctamente | ≤1 respuesta correcta o superficial |

---

*Basado en: MuseScore Studio 4 Handbook — Tablature, Fretboard diagrams | https://handbook.musescore.org*
