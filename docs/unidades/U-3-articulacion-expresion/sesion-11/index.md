# Sesión 11: Líneas, octavas y notaciones de interpretación

📚 Handbook → Notation: Lines, Octave lines, Arpeggios and glissandi, Breaths and pauses | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="linea"></a> **Línea (line)** | Elemento gráfico que se extiende sobre un rango de notas o compases. A diferencia de un símbolo puntual, una línea afecta a todo el pasaje que cubre. Las líneas pueden tener función visual, de reproducción, o ambas. |
    | <a id="ligadura-fraseo"></a> **Ligadura de fraseo (slur)** | Línea curva que agrupa varias notas indicando que deben tocarse de forma ligada (*legato*), sin separación. Es una de las líneas más usadas en notación. No debe confundirse con la ligadura de prolongación. |
    | <a id="8va"></a> **8va (octava alta / ottava alta)** | Línea con el texto `8va` que indica que las notas bajo su alcance deben ejecutarse una octava por encima de lo escrito. Se coloca sobre el pentagrama. Atajo: `Ctrl + Alt + ↑` (en algunas configuraciones). |
    | <a id="8vb"></a> **8vb (octava baja / ottava bassa)** | Línea con el texto `8vb` (o `8va bassa`) que indica que las notas deben ejecutarse una octava por debajo de lo escrito. Se coloca debajo del pentagrama. Útil para evitar líneas adicionales en pasajes muy graves o agudos. |
    | <a id="15ma"></a> **15ma (quinceava / doble octava)** | Similar a la 8va pero indica dos octavas de diferencia. `15ma alta` (sobre el pentagrama) = dos octavas arriba; `15ma bassa` (debajo) = dos octavas abajo. |
    | <a id="glissando"></a> **Glissando** | Línea recta u ondulada entre dos notas de diferente altura. Indica que el intérprete debe deslizarse de una nota a la otra pasando por todas las alturas intermedias. En el piano se ejecuta arrastrando el dedo por las teclas blancas (o blancas y negras, según la indicación). |
    | <a id="arpegio"></a> **Arpegio (arpeggio)** | Línea vertical ondulada que se coloca delante de un acorde. Indica que las notas del acorde deben ejecutarse de forma sucesiva (de grave a aguda, o viceversa) y no simultáneamente. |
    | <a id="pedal"></a> **Línea de pedal (pedal line)** | Línea horizontal que se coloca debajo del pentagrama de piano con los símbolos *Ped.* al inicio y `*` al final (o `❬` en notación moderna). Indica el uso del pedal de resonancia: al inicio se presiona, al final se levanta. |
    | <a id="respiracion"></a> **Respiración / pausa (breath / pause / caesura)** | Símbolo que indica una breve interrupción del sonido o una respiración. En MuseScore, se encuentra en la paleta **Respiraciones y pausas**. El símbolo más común es la coma de respiración (`'`) o la cesura (`//`). |
    | <a id="anclaje"></a> **Anclaje (anchor)** | Puntos de inicio y fin de una línea que determinan a qué nota, compás o silencio está "anclada" la línea. Si movemos la nota, la línea se mueve con ella. El anclaje se muestra con tiradores (cuadrados pequeños) al seleccionar la línea. |
    | <a id="trino-linea"></a> **Línea de trino (trill line)** | Extensión del símbolo `tr` que se prolonga sobre varias notas con una línea ondulada. Se encuentra en la paleta **Líneas**, no en Ornamentos. Se aplica como cualquier línea: seleccionar nota inicial, `Shift + clic` en nota final, clic en la línea de trino. |

???+ note "Líneas: concepto, aplicación y edición"

    Las líneas son objetos que se extienden horizontalmente en la partitura y afectan a todas las notas dentro de su rango. Están agrupadas en la paleta **Líneas** de MuseScore.

    ### ¿Qué tipos de líneas existen?

    | Categoría | Ejemplos | ¿Afecta la reproducción? |
    |---|---|---|
    | **Expresión** | Ligadura de fraseo, línea de trino | Sí (legato, trino continuo) |
    | **Registro** | 8va, 8vb, 15ma, 15ma bassa | Sí (transpone la octava en reproducción) |
    | **Técnica instrumental** | Glissando, arpegio, pedal | Sí (glissando, arpegio, pedal) |
    | **Texto continuo** | *cresc.*, *dim.*, *rit.*, *accel.* | Sí (cambios graduales) |
    | **Visual** | Línea de corchete (bracket) | No (solo agrupación visual) |

    ### Aplicar una línea desde la paleta

    **Método de rango (recomendado):**
    1. Seleccionar la nota donde comienza la línea.
    2. Mantener `Shift` y hacer clic en la nota donde termina la línea.
    3. Ir a la paleta **Líneas** y hacer clic en la línea deseada.

    **Método directo:**
    1. Seleccionar la nota inicial.
    2. Hacer clic en la línea desde la paleta.
    3. La línea se aplica inicialmente con una longitud predeterminada (generalmente hasta la nota siguiente).
    4. Seleccionar el tirador final y arrastrarlo hasta la nota de destino, o usar `Shift + →` para extenderla.

    > Insertar captura de la paleta de Líneas con todos los tipos visibles: ligaduras, 8vas, glissandi, arpegios, pedal, trinos, *cresc.*, *dim.*, etc.

    ### Editar la extensión de una línea

    Al seleccionar una línea, aparecen **tiradores** (cuadrados pequeños) en sus extremos:
    - Arrastrar un tirador horizontalmente para extender o acortar la línea.
    - La línea permanece anclada a las notas de inicio y fin.
    - Para cambiar el anclaje (que comience o termine en otra nota): seleccionar el tirador y presionar `Shift + →` o `Shift + ←` para moverlo nota por nota.

    ### Propiedades de las líneas

    Seleccionando una línea, en el panel **Propiedades** se puede ajustar:
    - **Texto**: editar el texto que muestra la línea (ej. cambiar "8va" por "ottava").
    - **Estilo de línea**: sólida, punteada, con guiones, ondulada (según el tipo).
    - **Posición vertical**: arriba o abajo del pentagrama.
    - **Reproducción**: activar o desactivar el efecto sonoro de la línea (útil cuando la línea es solo visual).

    !!! tip "¿Línea visual o línea con reproducción?"
        No todas las líneas producen un cambio en el sonido. Por ejemplo, una ligadura de fraseo SÍ afecta la reproducción (las notas suenan legato), mientras que una línea de corchete NO (solo agrupa visualmente). Verificá siempre en el panel **Propiedades → Reproducción** si la línea tiene efecto sonoro activado.

???+ note "Líneas de octava: 8va, 8vb y 15ma"

    Las líneas de octava permiten escribir notas en un registro cómodo dentro del pentagrama mientras indican que deben sonar una o dos octavas desplazadas. Son esenciales para pasajes extremadamente agudos o graves.

    ### Tipos de líneas de octava

    | Símbolo | Significado | Colocación | Efecto |
    |---|---|---|---|
    | **8va** (ottava alta) | Una octava arriba | Sobre el pentagrama | Las notas suenan 8ª superior a lo escrito |
    | **8vb** (ottava bassa) | Una octava abajo | Debajo del pentagrama | Las notas suenan 8ª inferior a lo escrito |
    | **15ma alta** | Dos octavas arriba | Sobre el pentagrama | Las notas suenan 16ª superior |
    | **15ma bassa** | Dos octavas abajo | Debajo del pentagrama | Las notas suenan 16ª inferior |

    ### Insertar una línea de 8va

    1. Seleccionar la nota donde debe comenzar la octava.
    2. `Shift + clic` en la nota donde debe terminar.
    3. Desde la paleta **Líneas**, hacer clic en **8va** (ottava alta).
    4. La línea se dibuja sobre el pentagrama con el texto `8va` y una línea punteada o discontinua que indica el alcance.

    Para **8vb (octava baja)**:
    - Usar el símbolo **8vb** (o **8va bassa**) de la paleta **Líneas**. Se coloca automáticamente debajo del pentagrama.

    Para **15ma**:
    - Usar el símbolo **15ma alta** o **15ma bassa** de la misma paleta.

    > Insertar captura de un pasaje de flauta con 8va sobre un grupo de notas agudas, mostrando la línea punteada con el texto `8va` y el tirador visible.

    ### Reproducción de las líneas de octava

    MuseScore reproduce automáticamente las notas en la octava correspondiente:
    - Notas bajo **8va** suenan una octava más aguda.
    - Notas bajo **8vb** suenan una octava más grave.
    - Notas bajo **15ma** suenan dos octavas desplazadas.

    Esto es muy útil para verificar que escribiste correctamente: si la línea de 8va está mal extendida y deja notas fuera, esas notas sonarán en la octava original y se notará auditivamente el error.

    ### ¿Cuándo usar líneas de octava y cuándo no?

    - **Usar 8va/8vb**: cuando un pasaje está consistentemente muy agudo o muy grave y querés evitar muchas líneas adicionales. El pentagrama se lee más fácil.
    - **NO usar 8va/8vb**: cuando son solo una o dos notas aisladas fuera del pentagrama. En ese caso, es preferible usar líneas adicionales. Las líneas de octava para notas sueltas confunden más de lo que ayudan.
    - **Duración mínima**: una línea de octava debe cubrir al menos un compás o una frase. No tiene sentido poner una 8va sobre dos corcheas.

    !!! warning "La 8va/8vb afecta la altura escrita para instrumentos transpositores"
        Si estás escribiendo para un instrumento transpositor (clarinete en Si♭, trompeta, saxofón) en **afinación de concierto**, la 8va se aplica sobre la altura de concierto. Al volver a **afinación escrita**, la línea de octava se mantiene en su posición. Verificá que el resultado tenga sentido en ambos modos.

???+ note "Arpegios y glissandos"

    Dos líneas muy usadas en música instrumental: el arpegio para acordes expandidos y el glissando para transiciones entre notas.

    ### Arpegio (arpeggio)

    El arpegio es una línea vertical ondulada que se coloca a la izquierda de un acorde. Indica que las notas no deben tocarse simultáneamente, sino una después de otra.

    **Cómo insertar un arpegio:**
    1. Seleccionar la cabeza de una nota cualquiera del acorde.
    2. Desde la paleta **Líneas**, hacer clic en el símbolo de **Arpegio** (línea ondulada vertical).
    3. El arpegio se coloca automáticamente abarcando todas las notas del acorde.

    **Opciones del arpegio en el panel Propiedades:**
    - **Dirección**: de grave a agudo (flecha hacia arriba), de agudo a grave (flecha hacia abajo), o sin flecha (dirección estándar de grave a agudo).
    - **Longitud**: el arpegio se ajusta automáticamente a la extensión vertical del acorde. Si hay notas en dos pentagramas (piano), usar el **arpegio de gran pentagrama** que cruza ambos.
    - **Extensión manual**: si el arpegio no cubre todo el acorde, arrastrar el tirador del extremo hasta la nota correspondiente.

    > Insertar captura de un acorde de cuatro notas con arpegio (dirección estándar) y un segundo acorde con arpegio hacia abajo, mostrando el panel de Propiedades.

    ### Arpegio entre pentagramas (cross-staff arpeggio)

    Para un arpegio que cruza los dos pentagramas de un piano:
    1. Seleccionar una nota del acorde del pentagrama inferior.
    2. Desde la paleta **Líneas**, hacer clic en el arpegio de gran pentagrama (arpegio con corchete vertical que conecta ambos pentagramas).
    3. El arpegio se extiende automáticamente desde la nota más grave del pentagrama inferior hasta la más aguda del superior.

    **En reproducción**, el arpegio se ejecuta con una ligera separación entre notas. La velocidad del arpegio se puede ajustar en el panel **Propiedades → Reproducción → Extensión de tempo** (Spread). Un valor de 0 reproduce el acorde simultáneamente; valores mayores (ej. 0.5, 1.0) retrasan progresivamente cada nota.

    ### Glissando

    El glissando es una línea recta u ondulada que conecta dos notas de diferente altura, indicando que se debe deslizar entre ellas.

    **Cómo insertar un glissando:**
    1. Seleccionar la nota de inicio.
    2. `Shift + clic` en la nota de destino.
    3. Desde la paleta **Líneas**, hacer clic en el glissando deseado:
       - **Glissando recto**: línea recta diagonal.
       - **Glissando ondulado** (wavy): línea ondulada que conecta las dos notas.

    **Propiedades del glissando:**
    - **Estilo**: recto u ondulado.
    - **Reproducción**: por defecto, el glissando SÍ tiene efecto sonoro. MuseScore interpola entre las dos alturas generando un barrido cromático. Se puede desactivar en Propiedades → Reproducción si solo se quiere el efecto visual.
    - **Texto**: se puede añadir texto como "gliss." o "port." sobre la línea.

    > Insertar captura de un glissando recto entre un Do4 y un Sol5, y un glissando ondulado entre un Mi4 y un La5, con el panel de Propiedades visible.

    ### Diferencia entre glissando, portamento y slide

    - **Glissando**: deslizamiento discreto (por semitonos o por teclas blancas). Típico del piano y el arpa.
    - **Portamento**: deslizamiento continuo sin escalones. Típico de la voz, el violín o el trombón.
    - **Slide**: en guitarra y bajo eléctrico, deslizamiento de un traste a otro indicado con una línea. Se encuentra en la paleta **Líneas** para instrumentos de cuerda pulsada.

    En MuseScore, el glissando reproduce un barrido cromático entre las dos notas. El efecto puede ser más o menos realista según la biblioteca de sonidos instalada (MS Basic vs. Muse Sounds).

    !!! tip "Glissando en piano: ¿teclas blancas o cromático?"
        Por defecto, MuseScore reproduce el glissando como cromático (todos los semitonos). Si querés un glissando solo sobre teclas blancas (más típico del piano), podés cambiar el estilo de reproducción en el panel **Propiedades → Reproducción → Tipo de glissando** (si está disponible en tu versión de MuseScore), o ajustarlo manualmente con notas ocultas.

???+ note "Líneas de pedal (piano)"

    El pedal de resonancia (también llamado pedal *forte* o derecho) es fundamental en la escritura para piano. MuseScore ofrece una línea específica para indicarlo.

    ### Insertar una línea de pedal

    1. Seleccionar la nota donde se presiona el pedal.
    2. `Shift + clic` en la nota donde se levanta el pedal.
    3. Desde la paleta **Líneas**, hacer clic en **Pedal** (tiene el texto *Ped.*).

    La línea se coloca debajo del pentagrama inferior del piano y muestra:
    - Inicio: *Ped.* (o `❬` en notación moderna).
    - Fin: `*` (levantar pedal) o `❭`.
    - Opcional: línea horizontal entre ambos, o ángulos `❬____❭` que indican el momento de levantar y volver a pisar.

    > Insertar captura de una línea de pedal debajo de un pentagrama de piano, mostrando *Ped.* al inicio, la línea horizontal y el `*` al final.

    ### Estilos de notación de pedal

    MuseScore ofrece varios estilos de línea de pedal en la paleta **Líneas**:
    - **Pedal clásico**: *Ped.* ... `*` con línea horizontal.
    - **Pedal moderno**: `❬____❭` (símbolos de soporte angular) con o sin línea.
    - **Pedal con cambio por armonía**: `❬____❭` repetidos para cada cambio armónico.

    El estilo se elige desde la paleta. Una vez insertado, se puede cambiar el estilo en el panel **Propiedades**.

    ### Reproducción del pedal

    En MuseScore, la línea de pedal SÍ afecta la reproducción: las notas bajo el pedal resuenan más (emulando el efecto del pedal de resonancia). Sin embargo, la calidad de esta simulación depende de la biblioteca de sonidos:
    - **MS Basic**: efecto básico, puede sonar "embarrado" si el pedal cubre muchos cambios armónicos.
    - **Muse Sounds (Muse Keys)**: simulación mucho más realista del comportamiento del pedal de piano.

    !!! warning "Cuidado con los cambios armónicos bajo el pedal"
        En un piano real, mantener el pedal durante un cambio de acorde produce una mezcla de armonías que puede sonar desagradable. En la notación, la línea de pedal debe levantarse (`*`) antes de cada cambio armónico y volver a pisarse inmediatamente. En MuseScore, aunque la línea sea continua, el motor de reproducción puede interpretar los cambios si usás Muse Sounds.

???+ note "Respiraciones, pausas y cesuras"

    Las respiraciones y pausas son marcas que indican una interrupción breve del sonido. Se encuentran en la paleta **Respiraciones y pausas** (*Breaths and pauses*).

    ### Tipos de símbolos de respiración y pausa

    | Símbolo | Nombre | Significado |
    |---|---|---|
    | `'` | **Coma de respiración** (breath mark / *Luftpause*) | Breve pausa para tomar aire o separar frases. No interrumpe el pulso general. |
    | `//` | **Cesura** (caesura / *railroad tracks*) | Interrupción más marcada que la coma de respiración. Indica una pausa breve pero perceptible. |
    | **Calderón sobre barra de compás** | **Fermata sobre compás** (fermata on barline) | El calderón colocado sobre una barra de compás (no sobre una nota) indica un silencio prolongado entre secciones. |

    ### Insertar una respiración o pausa

    1. Seleccionar la nota o barra de compás donde se desea insertar.
    2. Ir a la paleta **Respiraciones y pausas**.
    3. Hacer clic en el símbolo deseado.

    Por defecto, estos símbolos NO afectan la reproducción (son principalmente visuales). Sin embargo, en **Propiedades** se puede activar el efecto de "pausa" ajustando la duración de la interrupción en milisegundos.

    > Insertar captura de una coma de respiración colocada entre dos frases de una melodía de viento, y una cesura entre dos secciones contrastantes.

    ### Respiraciones en instrumentos de viento y canto

    En partituras para instrumentos de viento o voz, las comas de respiración son importantes porque indican al intérprete dónde puede respirar sin romper el fraseo musical. Una coma de respiración mal colocada (en medio de una palabra o de una idea musical) puede arruinar la interpretación.

    En MuseScore, las respiraciones se colocan automáticamente sobre la barra de compás o sobre el pentagrama, según la configuración de estilo.

    !!! tip "Coma de respiración vs. cesura: ¿cuál usar?"
        - **Coma de respiración**: pausa muy breve, casi imperceptible. El pulso continúa. Úsala para que el intérprete "respire" entre frases.
        - **Cesura**: pausa más larga y deliberada. El pulso se interrumpe momentáneamente. Úsala entre secciones muy contrastantes o antes de un cambio drástico de tempo o carácter.

???+ note "Diferencia entre función visual y efecto de reproducción"

    Una distinción fundamental al trabajar con líneas en MuseScore: no todas las líneas "suenan". Algunas son puramente visuales.

    ### ¿Cómo saber si una línea afecta la reproducción?

    Seleccioná la línea y revisá el panel **Propiedades**. Si aparece una sección llamada **Reproducción** o un interruptor de reproducción, la línea tiene efecto sonoro.

    ### Líneas con efecto de reproducción

    | Línea | Efecto sonoro |
    |---|---|
    | Ligadura de fraseo | Reproduce las notas en *legato* (transiciones suaves) |
    | Línea de trino | Reproduce el trino sobre todo el rango cubierto |
    | 8va / 8vb / 15ma | Transpone la reproducción una o dos octavas |
    | Glissando | Reproduce un barrido cromático entre las notas |
    | Arpegio | Las notas suenan en secuencia, no simultáneamente |
    | Pedal | Emula la resonancia del pedal de piano |
    | *cresc.* / *dim.* | Cambio gradual de volumen |
    | *rit.* / *accel.* | Cambio gradual de tempo |

    ### Líneas sin efecto de reproducción (solo visuales)

    | Línea | Función |
    |---|---|
    | Corchete / llave (bracket/brace) | Agrupación visual de pentagramas. No afecta el sonido. |
    | Línea de texto simple | Solo muestra texto. |
    | Algunas líneas de pedal (según configuración) | Si se desactiva la reproducción, son solo visuales. |

    ### Activación y desactivación de la reproducción

    En cualquier línea que tenga efecto sonoro, se puede desactivar la reproducción desde el panel **Propiedades → Reproducción**. Esto puede ser útil cuando:
    - Estás usando una línea de 8va como ayuda visual para el director, pero querés que el pentagrama suene en la octava escrita.
    - Estás usando un glissando como indicación de interpretación, pero no querés que el MIDI lo reproduzca.
    - Estás preparando una partitura para un examen donde el efecto sonoro podría confundir la revisión.

    !!! warning "No confundir silencio con error de notación"
        Si una línea de 8va no está produciendo el cambio de octava esperado, antes de asumir que es un bug de MuseScore, verificá que la reproducción esté activada en el panel **Propiedades**. Muchas veces el problema es simplemente que la reproducción se desactivó accidentalmente.

---

## Actividad en Classroom

### Tarea: S11 — Líneas, octavas y notaciones de interpretación

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S11_lineas.mscz`, una partitura para piano (gran pentagrama) en Fa mayor, 4/4, 24 compases con una pieza breve sin líneas de octava, glissandos, arpegios ni pedal; (b) `ejercicio_S11_vientos.mscz`, una partitura para cuarteto de vientos (flauta, oboe, clarinete en Si♭, fagot) en Sol mayor, 3/4, 16 compases con pasajes melódicos que se beneficiarían de indicaciones de respiración y octava.

1. **Líneas de octava.** Abrí `ejercicio_S11_lineas.mscz`. La pieza de piano contiene pasajes agudos en la mano derecha que exceden el pentagrama y pasajes graves en la mano izquierda con muchas líneas adicionales:
    - Identificá al menos 2 frases donde una **8va** (ottava alta) mejoraría la legibilidad de la mano derecha. Insertalas sobre el pentagrama superior usando el método de selección con rango (`Shift + clic` en nota final).
    - Identificá al menos 1 frase donde una **8vb** (ottava bassa) sea útil para la mano izquierda. Insertala debajo del pentagrama inferior.
    - Reproducí y verificá que las notas bajo las líneas de octava suenen en la octava correcta.

2. **Arpegios.** En la misma partitura de piano:
    - Localizá los acordes en los compases indicados por el docente (al menos 3 acordes de 3 o 4 notas).
    - Insertá un **arpegio** en cada uno. Probá diferentes direcciones: al menos uno estándar (grave a agudo), uno con flecha hacia abajo (agudo a grave).
    - Buscá un acorde que abarque ambos pentagramas (mano derecha e izquierda simultáneamente). Insertá un **arpegio de gran pentagrama** (cross-staff) que conecte ambos.
    - Ajustá la velocidad del arpegio en el panel **Propiedades → Reproducción → Extensión de tempo** (Spread). Probá valores de 0.3, 0.7 y 1.2. ¿Cuál suena más natural?

3. **Glissandos.** En la misma partitura de piano:
    - Identificá al menos 2 pares de notas donde un glissando tenga sentido musical (notas separadas por intervalo amplio, al menos una quinta).
    - Insertá un **glissando recto** y un **glissando ondulado** (wavy) en pares distintos.
    - Reproducí y compará: ¿se nota diferencia entre el recto y el ondulado en la reproducción?
    - Activá y desactivá la reproducción del glissando desde el panel **Propiedades**. ¿En qué caso conviene tener la reproducción activada? ¿Y desactivada?

4. **Pedal de piano.** En la misma partitura de piano (`ejercicio_S11_lineas.mscz`):
    - Insertá al menos 3 líneas de **pedal** debajo del pentagrama inferior, cubriendo frases de 2 a 4 compases cada una.
    - Usá el estilo clásico (*Ped.* ... `*`) en dos de ellas.
    - Probá el estilo moderno (`❬____❭`) en la tercera.
    - Escuchá atentamente la reproducción: ¿el pedal embarra los cambios armónicos o los respeta?
    - Ajustá los puntos de levantamiento del pedal (`*`) para que coincidan con los cambios de armonía y evitá que dos acordes distintos resuenen simultáneamente.

5. **Respiraciones y pausas en ensamble de vientos.** Abrí `ejercicio_S11_vientos.mscz`:
    - Identificá las frases melódicas en cada instrumento. Insertá al menos 2 **comas de respiración** (breath mark) en cada pentagrama, en lugares donde un instrumentista de viento necesitaría tomar aire sin romper el fraseo.
    - Insertá al menos 1 **cesura** (`//`) entre dos secciones de la pieza que tengan un cambio de carácter o tempo.
    - Reproducí la partitura y verificá que las respiraciones no corten ideas musicales a la mitad. Si alguna coma de respiración está mal ubicada, movela.

6. **Análisis de función visual vs. reproducción.** Al finalizar todos los pasos:
    - Seleccioná cada tipo de línea que hayas insertado (8va, arpegio, glissando, pedal, respiración) y revisá el panel **Propiedades**.
    - Elaborá una lista (en un comentario de Classroom o en un archivo de texto) donde clasifiques cada línea según si su efecto es **visual**, **de reproducción** o **ambos**.
    - Para cada línea, indicá si tuviste que ajustar su reproducción (activándola, desactivándola o modificando parámetros).

### Entregables

- [ ] `APELLIDO_Nombre_S11_lineas_v01.mscz` (piano con 8vas, arpegios, glissandos, pedal)
- [ ] `APELLIDO_Nombre_S11_lineas_v01.pdf`
- [ ] `APELLIDO_Nombre_S11_vientos_v01.mscz` (cuarteto de vientos con respiraciones y cesuras)
- [ ] `APELLIDO_Nombre_S11_vientos_v01.pdf`
- [ ] Captura de pantalla de un arpegio de gran pentagrama con el panel de Propiedades visible (sección Reproducción)
- [ ] Lista de clasificación visual/reproducción (en comentario de Classroom)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Líneas de octava (8va/8vb) | ≥2 frases con 8va en mano derecha y ≥1 con 8vb en mano izquierda; reproducción correcta | 1–2 líneas de octava insertadas pero mal extendidas o sin verificación auditiva | Sin líneas de octava |
| Arpegios | ≥3 arpegios en acordes diferentes; al menos 1 cross-staff; velocidad ajustada | 2 arpegios o sin ajuste de velocidad | ≤1 arpegio o sin cross-staff |
| Glissandos | ≥2 glissandos (recto + ondulado) en pares de notas adecuados; reproducción comparada | 1 glissando o sin comparación auditiva | Sin glissandos |
| Pedal de piano | ≥3 líneas de pedal; estilos variados (clásico + moderno); levantamiento en cambios armónicos | 2 líneas o sin ajuste de cambios armónicos | ≤1 línea de pedal |
| Respiraciones y pausas | ≥2 comas de respiración por instrumento + ≥1 cesura; ubicación musicalmente lógica | Faltan respiraciones en algún pentagrama o ubicación dudosa | Sin respiraciones o cesura |
| Clasificación visual/reproducción | Lista completa y correcta; justifica cada clasificación | Lista parcial o con 1–2 errores de clasificación | No entregó la clasificación |

---

*Basado en: MuseScore Studio 4 Handbook — Lines, Octave lines, Arpeggios and glissandi, Breaths and pauses | https://handbook.musescore.org*
