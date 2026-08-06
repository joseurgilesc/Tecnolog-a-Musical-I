# Sesión 17: Acordes, cifrado y notación pianística

📚 Handbook → Text: Chord notation systems | Notation: Fretboard diagrams, Cross-staff notation | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="triada"></a> **Tríada (triad)** | Acorde de tres notas formado por superposición de terceras: fundamental, tercera (mayor o menor) y quinta (justa, disminuida o aumentada). Es la unidad básica de la armonía tonal. Los cuatro tipos son: mayor (3M + 5J), menor (3m + 5J), disminuido (3m + 5dim) y aumentado (3M + 5aum). |
    | <a id="cuatriada"></a> **Cuatríada (seventh chord)** | Acorde de cuatro notas que añade una séptima a la tríada base. Tipos principales: séptima dominante (3M + 5J + 7m), séptima mayor (3M + 5J + 7M), séptima menor (3m + 5J + 7m), semidisminuido (3m + 5dim + 7m), disminuido completo (3m + 5dim + 7dim). |
    | <a id="cifrado-americano"></a> **Cifrado americano (chord symbol)** | Sistema de notación abreviada para acordes usado en jazz, pop y música popular. La letra mayúscula indica la fundamental (C = Do, D = Re), seguida de la cualidad (m = menor, maj7 = séptima mayor, dim = disminuido) y extensiones (9, 11, 13). El bajo alterado se indica con barra: C/E = Do mayor con Mi en el bajo. Se ingresa con `Ctrl + K`. |
    | <a id="bajo-cifrado"></a> **Bajo cifrado (figured bass)** | Sistema de notación del Barroco (siglos XVII–XVIII) donde la armonía se indica con números bajo la línea del bajo. El intérprete "realiza" el cifrado improvisando las voces superiores. Los números indican intervalos sobre el bajo: 6 = primera inversión, 6/4 = segunda inversión, 7 = séptima. Una ausencia de números implica tríada en estado fundamental (5/3, que se omite). |
    | <a id="cross-staff"></a> **Notación cruzada (cross-staff notation)** | Técnica pianística donde las notas de un pentagrama "cruzan" visualmente al otro pentagrama para reflejar cómo se tocan con una sola mano. Ejemplo: una línea melódica en el pentagrama inferior que en realidad la toca la mano derecha cruzando sobre la izquierda. En MuseScore se logra moviendo notas entre pentagramas con `Ctrl + Shift + ↑ / ↓`. |
    | <a id="inversion"></a> **Inversión (inversion)** | Posición de un acorde determinada por la nota que está en el bajo. Estado fundamental: fundamental en el bajo. Primera inversión: tercera en el bajo. Segunda inversión: quinta en el bajo. Tercera inversión (solo cuatríadas): séptima en el bajo. El cifrado americano indica la inversión con barra (C/E), el bajo cifrado con números (6, 6/4). |
    | <a id="voicing"></a> **Voicing / Disposición** | Distribución concreta de las notas de un acorde entre las voces o entre las manos del pianista. Un mismo acorde C (Do-Mi-Sol) puede tocarse en posición cerrada (notas juntas), abierta (notas espaciadas), con duplicaciones, u omitiendo la quinta. La notación pianística profesional refleja el *voicing* elegido. |
    | <a id="plicas-cruzadas"></a> **Plicas en notación cruzada** | Cuando una voz cruza de un pentagrama a otro en notación de piano, las plicas mantienen la dirección de la voz original. Si la voz pertenece a la mano derecha (plica arriba) pero sus notas caen en el pentagrama inferior, las plicas SIGUEN apuntando hacia arriba para indicar continuidad de la voz. |
    | <a id="acorde-extendido"></a> **Acorde extendido (extended chord)** | Acorde que añade tensiones más allá de la séptima: novena (9), oncena (11), trecena (13). Se notan en cifrado americano: Cmaj9, Dm11, G13. En notación de piano, las tensiones suelen escribirse en la mano derecha mientras la mano izquierda toca las notas guía (fundamental, tercera, séptima). |
    | <a id="notas-guia"></a> **Notas guía (guide tones)** | La tercera y la séptima de un acorde. Son las notas que definen la cualidad del acorde (mayor/menor/dominante). En arreglos de piano y big band, las notas guía suelen tocarse en un registro medio mientras la melodía y las tensiones van en registros superiores. La fundamental y la quinta son opcionales porque no definen la "personalidad" del acorde. |
    | <a id="pedal-armonico"></a> **Pedal armónico (pedal point)** | Nota sostenida (generalmente el bajo) sobre la cual cambian los acordes superiores. Crea tensión armónica porque los acordes superiores pueden ser disonantes con el pedal. En notación de piano, el pedal se escribe como una nota larga (redonda o blanca) en el pentagrama inferior mientras los acordes cambian encima. |
    | <a id="enarmonia"></a> **Enarmonía (enharmonic)** | Dos notas que suenan igual pero se escriben diferente: Do♯ = Re♭, Sol♯ = La♭. En cifrado armónico, elegir la enarmonía correcta es crucial para la legibilidad: C♯m es preferible a D♭m en tonalidades con sostenidos. El bajo cifrado usa la enarmonía que mejor refleje la función armónica, no necesariamente la más "fácil de leer". |

???+ note "Acordes y tríadas: de la teoría al pentagrama"

    Antes de escribir cifrado, hay que ENTENDER qué hay dentro del acorde. Un cifrado es una etiqueta. El acorde real son las notas que suenan.

    ### La tríada: el ladrillo de la armonía

    Una tríada se construye apilando dos terceras sobre una nota base (fundamental):

    ```
    Fundamental → +3ª → +3ª (→ quinta)
       Do    →   Mi  →  Sol   = Do mayor (C)
       La    →   Do  →  Mi    = La menor (Am)
    ```

    Los cuatro tipos de tríada y su "fórmula de terceras":

    | Tipo | Fórmula | Ejemplo (desde Do) | Cifrado |
    |---|---|---|---|
    | **Mayor** | 3ª mayor + 3ª menor | Do–Mi–Sol | C |
    | **Menor** | 3ª menor + 3ª mayor | Do–Mi♭–Sol | Cm |
    | **Disminuido** | 3ª menor + 3ª menor | Do–Mi♭–Sol♭ | Cº o Cdim |
    | **Aumentado** | 3ª mayor + 3ª mayor | Do–Mi–Sol♯ | C+ o Caug |

    ### Cómo escribir tríadas en MuseScore

    1. Ingresar la fundamental (ej. Do) en modo de ingreso de notas (`N`).
    2. Para agregar la tercera: seleccionar el Do, presionar `Alt + 3` (intervalo de tercera arriba). MuseScore agrega un Mi.
    3. Para agregar la quinta: con el Mi aún seleccionado (o ambos), `Alt + 3` otra vez → Sol.
    4. O alternativamente: ingresar Do, luego `Shift + E` y `Shift + G` para agregar notas simultáneas en el mismo tiempo.

    !!! tip "Escuchar antes de escribir"
        Cuando ingreses un acorde en el pentagrama, reproducilo inmediatamente. ¿Suena como esperabas? Si escribiste C (Do mayor) y suena "triste", probablemente ingresaste Mi♭ en lugar de Mi natural. La teoría sin oído es caligrafía, no música.

    ### Inversiones de tríadas en el pentagrama

    | Inversión | Bajo | Apariencia en el pentagrama | Cifrado americano |
    |---|---|---|---|
    | **Estado fundamental** | Fundamental (Do) | Do–Mi–Sol (terceras apiladas) | C |
    | **Primera inversión** | Tercera (Mi) | Mi–Sol–Do (tercera + cuarta) | C/E |
    | **Segunda inversión** | Quinta (Sol) | Sol–Do–Mi (cuarta + tercera) | C/G |

    En el piano, las inversiones se escriben con la nota del bajo en el pentagrama inferior y el resto del acorde en el superior. La nota después de la barra (C/E) indica qué nota debe tocar la mano izquierda.


???+ note "Cifrado americano avanzado: más allá de la tríada"

    El cifrado básico (C, Am, G7) lo viste en la Sesión 14. Ahora expandimos a cuatríadas, acordes extendidos y notación profesional de jazz.

    ### Séptimas: la cuarta nota que cambia todo

    | Tipo | Fórmula (desde Do) | Notas | Cifrado | Se usa en... |
    |---|---|---|---|---|
    | **7 dominante** | 3M + 5J + 7m | Do–Mi–Sol–Si♭ | C7 | Blues, funk, V7 clásico |
    | **7 mayor** | 3M + 5J + 7M | Do–Mi–Sol–Si | Cmaj7, CΔ | Jazz, bossa nova, pop sofisticado |
    | **7 menor** | 3m + 5J + 7m | Do–Mi♭–Sol–Si♭ | Cm7, C-7 | ii en ii-V-I, funk, soul |
    | **Semidisminuido** | 3m + 5dim + 7m | Do–Mi♭–Sol♭–Si♭ | Cm7♭5, Cø | viiø7 en tonalidad menor, jazz |
    | **Disminuido 7** | 3m + 5dim + 7dim | Do–Mi♭–Sol♭–Si♭♭ (La) | Cº7, Cdim7 | Tonalidad menor, cromatismo |

    ### Cómo ingresar cifrado avanzado en MuseScore

    Activá `Ctrl + K` sobre la nota donde empieza el acorde y escribí:

    | Lo que escribís | Lo que MuseScore muestra | El acorde |
    |---|---|---|
    | `Cmaj7` | Cmaj7 | Do mayor séptima mayor |
    | `C7` | C7 | Do dominante (séptima) |
    | `Cm7` | Cm7 | Do menor séptima |
    | `Cm7b5` | Cm7♭5 | Do semidisminuido |
    | `Co` (letra o minúscula) | Cº | Do disminuido (tríada) |
    | `C/E` | C/E | Do mayor con Mi en el bajo |
    | `C7/E` | C7/E | Do dominante con Mi en el bajo |
    | `Cmaj9` | Cmaj9 | Do mayor séptima mayor con novena |
    | `Dm11` | Dm11 | Re menor con oncena |

    !!! tip "El símbolo delta Δ y otros atajos"
        En partituras de jazz manuscritas se usa Δ para maj7 (CΔ = Cmaj7) y − para menor (C−7 = Cm7). MuseScore entiende ambos al ingresar el cifrado. Escribí `Cma7` o `Ct` (triángulo) según prefieras. Lo importante es la CONSISTENCIA: no mezcles Δ y maj7 en la misma partitura.

    ### Acordes extendidos: 9, 11, 13

    - **Novena (9)**: añade la 9ª sobre la fundamental. C9 = Do–Mi–Sol–Si♭–Re. Si el acorde NO tiene séptima se escribe Cadd9.
    - **Oncena (11)**: añade la 11ª (cuarta). Cm11 = Do–Mi♭–Sol–Si♭–Re–Fa (generalmente se omite la 3ª para evitar choque con la 11ª).
    - **Trecena (13)**: añade la 13ª (sexta). C13 = Do–Mi–Sol–Si♭–Re–(Fa)–La. Las notas intermedias (9, 11) son opcionales en la ejecución.

    En la práctica pianística, los acordes extendidos rara vez se tocan con TODAS las notas. La regla profesional:
    - **Mano izquierda**: fundamental + séptima (o fundamental + quinta).
    - **Mano derecha**: tercera + séptima + tensiones (9, 11, 13) en la octava adecuada.


???+ note "Bajo cifrado: el lenguaje armónico del Barroco"

    Antes del cifrado americano, existió el bajo cifrado. Si bien hoy es histórico, entenderlo te da una comprensión más profunda de cómo funciona la armonía y por qué ciertas inversiones se llaman "acorde de sexta" o "de cuarta y sexta".

    ### Cómo funciona

    El bajo cifrado es un sistema de números escritos DEBAJO de las notas del bajo que indican los intervalos que deben tocarse SOBRE esa nota del bajo:

    | Cifrado | Intervalos sobre el bajo | Inversión resultante | Ejemplo (bajo = Do) |
    |---|---|---|---|
    | *(sin números)* | 5ª y 3ª (implícito) | Estado fundamental | Do–Mi–Sol (C) |
    | 6 | 6ª (y 3ª implícita) | Primera inversión | Do–Mi♭–La♭ (La♭/Do, o sea A♭/C) |
    | 6/4 | 6ª y 4ª | Segunda inversión | Do–Fa–La (Fa/Do, o sea F/C) |
    | 7 | 7ª, 5ª y 3ª | Séptima en estado fundamental | Do–Mi–Sol–Si♭ (C7) |
    | 6/5 | 6ª y 5ª (y 3ª) | Séptima en primera inversión | Do–Mi–Sol–La (Am7/C) |
    | 4/3 | 4ª y 3ª (y 6ª implícita) | Séptima en segunda inversión | Do–Mi–Fa–La (Fmaj7/C) |
    | 4/2 (o 2) | 4ª y 2ª (y 6ª) | Séptima en tercera inversión | Do–Re–Fa–La (Dm7/C) |

    ### Alteraciones en el bajo cifrado

    Una alteración (♯, ♭, ♮) al lado de un número indica que ESE intervalo se altera:
    - ♯6 = la sexta sobre el bajo es ascendida medio tono.
    - ♭5 = la quinta sobre el bajo es descendida medio tono.
    - Una alteración SOLA (sin número) se aplica a la tercera.


    ### ¿Por qué aprender bajo cifrado si no se usa hoy?

    1. **Comprensión de inversiones**: el bajo cifrado te obliga a pensar en intervalos desde el bajo, que es exactamente lo que hace el oído para reconocer inversiones.
    2. **Lectura de partituras históricas**: si alguna vez tocás una edición Urtext de Bach o Händel, el continuo está en bajo cifrado.
    3. **Teoría de la armonía**: muchos conceptos de armonía moderna (cifrado funcional con números romanos: I, IV, V, ii, vi) heredan directamente la lógica del bajo cifrado.

    !!! warning "No confundir bajo cifrado con cifrado americano"
        C/E en cifrado americano = Do mayor con Mi en el bajo. Especifica la nota EXACTA del bajo.
        6 en bajo cifrado = "tocá una sexta y una tercera sobre esta nota del bajo". No especifica la fundamental del acorde: el intérprete tiene que deducirla.
        Son sistemas distintos con propósitos distintos. El americano te dice QUÉ acorde es. El barroco te dice QUÉ intervalos construir.

???+ note "Notación pianística: cross-staff y voicing profesional"

    La notación para piano tiene convenciones propias que van más allá de "melodía arriba, acompañamiento abajo". Las partituras pianísticas profesionales comunican digitación, distribución entre manos y voicing a través de la posición visual de las notas.

    ### Cross-staff: cuando las notas cruzan pentagramas

    En el piano, las dos manos no siempre tocan lo que está en "su" pentagrama. Una melodía en la mano derecha puede bajar al pentagrama inferior, y un bajo en la mano izquierda puede subir al pentagrama superior. La notación **cross-staff** refleja esta realidad física.

    **Cómo hacer cross-staff en MuseScore:**

    1. Ingresar las notas en el pentagrama de origen (donde empiezan).
    2. Seleccionar las notas que deben cruzar al otro pentagrama.
    3. Presionar `Ctrl + Shift + ↑` (subir al pentagrama superior) o `Ctrl + Shift + ↓` (bajar al pentagrama inferior).
    4. Las notas se mueven visualmente al otro pentagrama pero MANTIENEN su pertenencia original (plicas, silencios, etc.).

    **Indicador visual**: las notas en cross-staff mantienen las plicas apuntando hacia el pentagrama de origen. Si una nota de la mano derecha cae en el pentagrama inferior, sus plicas apuntarán hacia arriba (dirección de la mano derecha).


    ### Voicing pianístico: distribución de notas entre manos

    | Situación | Mano izquierda | Mano derecha |
    |---|---|---|
    | **Tríada en posición cerrada** | Fundamental | 3ª + 5ª |
    | **Tríada en posición abierta** | Fundamental + 5ª | 3ª (octava superior) |
    | **Séptima (jazz)** | Fundamental + 7ª (o 3ª + 7ª) | 3ª + 7ª + tensiones (o melodía) |
    | **Acorde con bajo pedal** | Pedal sostenido | Acordes cambiantes |
    | **Melodía con acompañamiento** | Bajo + acordes quebrados | Melodía |

    ### Múltiples voces en notación de piano

    El piano usa frecuentemente 2 voces por pentagrama:
    - **Mano derecha, voz 1 (plica arriba)**: melodía principal.
    - **Mano derecha, voz 2 (plica abajo)**: notas de relleno armónico o contramelodía.
    - **Mano izquierda, voz 1 (plica abajo)**: bajo.
    - **Mano izquierda, voz 2 (plica arriba)**: acordes o notas tenidas.

    !!! tip "La regla de las plicas en piano"
        En un pentagrama de piano, la dirección de la plica comunica qué mano toca qué, incluso cuando las notas están en el mismo pentagrama. Si ves plicas arriba y abajo en el pentagrama superior, estás viendo dos capas: la melodía (plica arriba) y las notas de relleno (plica abajo). No son "errores": son voicing intencional.


    ### Silencios en notación de piano

    En partituras de piano con múltiples voces:
    - Cada voz tiene sus propios silencios.
    - Si una voz no suena en un compás, DEBE mostrar un silencio (típicamente una pausa de redonda en la posición adecuada).
    - Los silencios de voces secundarias se pueden ocultar seleccionándolos y presionando `V` (toggle de visibilidad), pero en general no se recomienda porque el intérprete pierde información sobre qué voces están activas.

---

## Actividad en Classroom

### Tarea: S17 — Acordes, cifrado y notación pianística

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S17_acordes.mscz`, una partitura para piano en Do mayor, 4/4, 16 compases con una melodía en el pentagrama superior y un bajo simple (redondas y blancas) en el inferior, SIN cifrado armónico y sin indicaciones de voicing; (b) `ejercicio_S17_bajocifrado.mscz`, una partitura para violonchelo solo en La menor, 4/4, 12 compases con una línea de bajo que podría ser la de un coral barroco, con espacio debajo para insertar el bajo cifrado; (c) `ejercicio_S17_crossstaff.mscz`, una partitura para piano en Sol mayor, 3/4, 20 compases con un pasaje melódico en la mano derecha que DESCIENDE hacia el pentagrama inferior y un acompañamiento quebrado en la mano izquierda, con las notas actualmente mal asignadas entre pentagramas.

1. **Construcción de acordes en el pentagrama.** Abrí `ejercicio_S17_acordes.mscz`:
    - Identificá la tonalidad y los grados armónicos que sugiere la línea del bajo.
    - En el pentagrama inferior, construí acordes completos (tríadas) sobre cada nota del bajo. Usá `Alt + 3` para agregar la tercera y la quinta.
    - Escribí al menos 8 acordes diferentes usando TODOS los tipos de tríada: mayor, menor, disminuido y aumentado (donde corresponda).
    - Asegurate de que las notas del acorde estén en el ámbito adecuado del pentagrama inferior (no uses notas demasiado agudas que "invadan" la melodía).
    - Ingresá el **cifrado americano** (`Ctrl + K`) sobre cada cambio de armonía. Verificá que el cifrado coincida exactamente con las notas que escribiste.

2. **Cifrado americano avanzado.** En el mismo archivo `ejercicio_S17_acordes.mscz` ya editado:
    - Transformá al menos 4 de las tríadas en **cuatríadas** (agregá la séptima correspondiente). Usá el `Alt + 3` para apilar una tercera adicional.
    - Actualizá el cifrado americano para reflejar las cuatríadas: Cmaj7, Dm7, G7, Am7, etc.
    - Ingresá al menos 3 acordes con **bajo alterado** (slash chords): C/E, F/A, G/B. Asegurate de que la nota del bajo en el pentagrama inferior coincida con la indicada después de la barra.
    - Ingresá al menos 2 acordes **extendidos** donde tenga sentido musical: Cmaj9, Dm11, G13, etc. No es necesario que escribas TODAS las notas del acorde extendido en el pentagrama (recordá la regla profesional: mano izq = notas guía, mano der = tensiones).
    - Reproducí la partitura. ¿La armonía que escuchás coincide con el cifrado que escribiste?

3. **Bajo cifrado: el laboratorio del Barroco.** Abrí `ejercicio_S17_bajocifrado.mscz`:
    - Analizá la línea del bajo. Determiná en qué grado de la escala está cada nota.
    - Insertá el **bajo cifrado** como texto de pentagrama (`Ctrl + T`) debajo de cada nota del bajo. Usá la notación numérica estándar: 6 para primera inversión, 6/4 para segunda inversión, 7 para séptimas, y alteraciones donde corresponda (♯3, ♭5, etc.).
    - Creá un NUEVO pentagrama de piano (gran pentagrama) en el mismo archivo. Andá a **Añadir → Instrumentos → Piano**.
    - Copiá la línea del bajo al pentagrama inferior del piano.
    - En el pentagrama superior del piano, "realizá" el bajo cifrado: escribí las voces superiores que completan la armonía indicada por el cifrado. Hacelo en estilo coral (4 voces, conducción suave de voces, sin saltos grandes entre una nota y la siguiente).
    - Reproducí la realización. ¿Suena como un coral barroco coherente?

4. **Notación cross-staff: arreglar el piano.** Abrí `ejercicio_S17_crossstaff.mscz`:
    - La partitura tiene un pasaje donde la melodía de la mano derecha desciende y "debería" tocarse con la mano derecha pero sus notas cayeron en el pentagrama inferior. Identificá esas notas.
    - Seleccioná las notas que pertenecen a la mano derecha pero están mal asignadas y movelas al pentagrama superior con `Ctrl + Shift + ↑`.
    - Revisá la dirección de las plicas: las notas que cross-staff deben mantener las plicas hacia arriba (dirección de mano derecha) aunque estén en el pentagrama inferior.
    - Identificá si hay notas en el pentagrama superior que en realidad las toca la mano izquierda (acompañamiento quebrado que "invade" el pentagrama superior). Movelas al pentagrama inferior con `Ctrl + Shift + ↓`.
    - Reproducí la pieza. Ahora debería ser más fácil de leer: cada mano tiene sus notas en el pentagrama correcto, independientemente de la altura absoluta.

5. **Integración: arreglo pianístico profesional.** Creá una NUEVA partitura desde cero: `APELLIDO_Nombre_S17_piano.mscz`.
    - Plantilla: Piano (gran pentagrama). Tonalidad: Mi bemol mayor (3 bemoles). Compás: 4/4. 24 compases.
    - **Estructura armónica obligatoria**: I (E♭) → vi (Cm7) → ii (Fm7) → V7 (B♭7) → I (E♭maj7). Desarrollá una progresión que use estos acordes en los primeros 8 compases y luego variaciones en los compases restantes.
    - **Melodía** (mano derecha, pentagrama superior): componé una melodía original de 24 compases usando valores de negra, corchea y blanca. Incluí al menos un tresillo.
    - **Acompañamiento** (mano izquierda, pentagrama inferior): escribí un acompañamiento con acordes en la mano izquierda usando voicings de jazz: fundamental + séptima en la mano izquierda, tercera + séptima + tensiones en la mano derecha.
    - **Cifrado americano**: ingresá el cifrado (`Ctrl + K`) sobre CADA cambio de armonía. Usá al menos: 2 acordes mayores, 2 menores, 2 séptimas dominantes, 2 séptimas mayores, 1 semidisminuido, 2 con bajo alterado (slash chords).
    - **Cross-staff**: en algún momento de la pieza (al menos 4 compases consecutivos), hacé que la mano derecha cruce al pentagrama inferior (melodía que baja) o que la mano izquierda cruce al pentagrama superior (bajo que sube). Usá `Ctrl + Shift + ↑ / ↓`.
    - **Bajo pedal**: en los últimos 4 compases, escribí un pedal de tónica (Mi♭ sostenido en el bajo) mientras los acordes superiores cambian arriba.
    - **Texto de interpretación**: agregá al menos 3 indicaciones de Staff Text: *cantabile* en la melodía, *legato* en el acompañamiento, y una indicación de dinámica (`p`, `mf`, `f`).
    - Exportá como PDF.

6. **Reflexión sobre armonía y notación.** En Classroom, respondé:
    - ¿Cuál es la diferencia práctica entre una tríada mayor y una cuatríada maj7? ¿Cómo cambia el "color" del acorde al agregar la séptima?
    - ¿Por qué el bajo cifrado usa números y no letras como el cifrado americano? ¿Qué ventajas y desventajas tiene cada sistema?
    - En la notación cross-staff, ¿por qué es importante que las plicas mantengan la dirección de la mano original aunque la nota esté en el otro pentagrama? ¿Qué pasaría si las plicas cambiaran de dirección?

### Entregables

- [ ] `APELLIDO_Nombre_S17_acordes_v01.mscz` (piano con acordes construidos + cifrado americano avanzado)
- [ ] `APELLIDO_Nombre_S17_acordes_v01.pdf`
- [ ] `APELLIDO_Nombre_S17_bajocifrado_v01.mscz` (bajo cifrado + realización para piano)
- [ ] `APELLIDO_Nombre_S17_bajocifrado_v01.pdf`
- [ ] `APELLIDO_Nombre_S17_crossstaff_v01.mscz` (cross-staff corregido)
- [ ] `APELLIDO_Nombre_S17_crossstaff_v01.pdf`
- [ ] `APELLIDO_Nombre_S17_piano_v01.mscz` (arreglo pianístico completo)
- [ ] `APELLIDO_Nombre_S17_piano_v01.pdf`
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) la progresión armónica que usaste en tu arreglo pianístico (escribila como secuencia de cifrados, ej. E♭maj7 → Cm7 → Fm7 → B♭7...)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Construcción de acordes | ≥8 acordes con tipos variados (M, m, dim, aum); notas correctas; ámbito adecuado en el pentagrama | 5–7 acordes correctos o poca variedad de tipos | ≤4 acordes o notas incorrectas |
| Cifrado americano avanzado | ≥4 cuatríadas, ≥3 slash chords, ≥2 acordes extendidos; todo el cifrado coincide con las notas | Cifrado presente pero con 2–3 errores de correspondencia cifrado-notas | Cifrado ausente o incorrecto en >50% |
| Bajo cifrado | Cifrado correcto según análisis; realización a 4 voces con conducción suave; suena como un coral coherente | Cifrado presente pero con errores de análisis; realización incompleta o con saltos grandes | Sin bajo cifrado o realización incoherente |
| Cross-staff | Notas reasignadas correctamente; plicas mantienen dirección original; la partitura es más legible | Reasignación parcial o algunas plicas incorrectas | Sin cambios o empeoró la legibilidad |
| Arreglo pianístico | Progresión I-vi-ii-V7-I presente; voicing profesional; cross-staff funcional; pedal armónico correcto; cifrado completo y variado | Arreglo presente pero falta algún elemento (voicing, cross-staff, pedal) | Arreglo incompleto o sin varios elementos obligatorios |
| Reflexión | Responde las 3 preguntas con comprensión; demuestra distinguir tríada/cuatríada, sistemas de cifrado y propósito del cross-staff | Responde 2 de 3 correctamente | ≤1 respuesta correcta o sin argumentación |

---

*Basado en: MuseScore Studio 4 Handbook — Chord notation systems, Cross-staff notation, Fretboard diagrams | https://handbook.musescore.org*
