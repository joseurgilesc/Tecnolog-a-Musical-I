# Sesión 10: Dinámicas, tempo y reproducción

📚 Handbook → Notation: Expressive markings — Dynamics and hairpins; Text — Tempo markings; Sound and Playback — Mixer, Playback controls | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="dinamica"></a> **Dinámica (dynamic)** | Indicación de la intensidad o volumen con que debe ejecutarse un pasaje musical. Se escribe con abreviaturas italianas: ***pp*** (pianissimo, muy suave), ***p*** (piano, suave), ***mp*** (mezzo-piano, medio suave), ***mf*** (mezzo-forte, medio fuerte), ***f*** (forte, fuerte), ***ff*** (fortissimo, muy fuerte). |
    | <a id="regulador"></a> **Regulador (hairpin)** | Símbolo gráfico en forma de ángulo que se abre `\<` (crescendo) o se cierra `\>` (diminuendo/decrescendo) para indicar un cambio gradual de intensidad. Atajo: `<` para crescendo, `>` para diminuendo. |
    | <a id="crescendo"></a> **Crescendo (cresc.)** | Aumento gradual de la intensidad. Puede indicarse con un regulador que se abre o con la abreviatura *cresc.* seguida de una línea punteada. |
    | <a id="diminuendo"></a> **Diminuendo / Decrescendo (dim. / decresc.)** | Disminución gradual de la intensidad. Se indica con un regulador que se cierra o con la abreviatura *dim.* seguida de una línea punteada. |
    | <a id="marca-tempo"></a> **Marca de tempo** | Indicación que establece la velocidad de la música. Puede ser una **marca metronómica** (♩ = 120), una **indicación verbal** (Allegro, Andante, Adagio) o una **modulación métrica** (♩ = ♩.). |
    | <a id="metronomo"></a> **Metrónomo (metronome)** | Herramienta que produce un pulso regular (clic) para mantener el tempo durante la práctica o la reproducción. En MuseScore, se activa con el botón del metrónomo en la barra de reproducción. |
    | <a id="cambio-tempo"></a> **Línea de cambio de tempo** | Línea con texto como *accel.* (accelerando), *rit.* (ritardando) o *rall.* (rallentando) que indica un cambio gradual de velocidad a lo largo de varios compases. En MuseScore, se encuentran en la paleta **Tempo**. |
    | <a id="mixer"></a> **Mixer / Mezclador** | Panel de MuseScore (`F10`) que permite ajustar el volumen, el paneo estéreo, el sonido (instrumento virtual), los efectos de audio y la reverberación de cada instrumento de la partitura de forma independiente. |
    | <a id="panel-reproduccion"></a> **Panel de reproducción (Playback toolbar)** | Barra de herramientas en la parte superior derecha de MuseScore que contiene los controles de reproducción: Play, Stop, Loop, Metrónomo, velocidad de reproducción y contadores de posición (tiempo / compases). |
    | <a id="cambio-sonido"></a> **Cambio de sonido a mitad de pentagrama (mid-score instrument change)** | Funcionalidad que permite cambiar el sonido de un instrumento en un punto específico de la partitura sin modificar la notación del pentagrama. Se usa para que un mismo pentagrama suene con diferentes instrumentos en secciones distintas. |

???+ note "Dinámicas: de pianissimo a fortissimo"

    Las dinámicas indican la **intensidad** con que se ejecuta un pasaje. Son uno de los recursos expresivos más poderosos en MuseScore porque el programa las reproduce automáticamente.

    ### Dinámicas básicas

    | Abreviatura | Significado | Intensidad relativa |
    |---|---|---|
    | ***ppp*** | Pianissimo possibile | Lo más suave posible |
    | ***pp*** | Pianissimo | Muy suave |
    | ***p*** | Piano | Suave |
    | ***mp*** | Mezzo-piano | Medio suave |
    | ***mf*** | Mezzo-forte | Medio fuerte |
    | ***f*** | Forte | Fuerte |
    | ***ff*** | Fortissimo | Muy fuerte |
    | ***fff*** | Fortissimo possibile | Lo más fuerte posible |

    ### Agregar una dinámica

    **Desde la paleta Dinámicas:**
    1. Seleccionar una o varias notas.
    2. Hacer clic en la dinámica deseada en la paleta **Dinámicas**.
    3. La dinámica se coloca automáticamente debajo del pentagrama asociada a esa nota.

    **Desde el popup de dinámicas:**
    1. Seleccionar una nota.
    2. Presionar `Ctrl + D` (`Cmd + D` en macOS). Aparece un popup con las dinámicas disponibles.
    3. Hacer clic en la deseada o escribir su abreviatura (ej. `pp`, `mf`, `ff`).


    ### Combinar dinámicas con texto

    MuseScore permite dos formas de combinar texto con dinámicas:
    - **Texto de expresión separado**: agregar la dinámica, luego agregar un texto de expresión desde la paleta **Texto** (ej. *dolce*, *espress.*). Ambos se alinean automáticamente.
    - **Texto dentro de la dinámica**: hacer doble clic en la dinámica y escribir el texto directamente (ej. *più **p***, ***f** sub.*). El texto se trata como parte del mismo elemento.

    !!! tip "Las dinámicas se heredan hasta la siguiente"
        En reproducción, una dinámica afecta a su voz asignada desde el punto donde aparece **hasta que otra dinámica la reemplace**. Si escribís ***f*** en el compás 1 y no ponés nada más, todo el resto de la partitura sonará fuerte. Siempre cerrá tus frases con una dinámica apropiada.

???+ note "Reguladores: crescendo y diminuendo"

    Los reguladores indican un **cambio gradual** de intensidad, a diferencia de las dinámicas que marcan un nivel fijo.

    ### Agregar un regulador

    **Con atajo de teclado (recomendado):**
    1. Seleccionar un rango de notas o compases.
    2. Presionar `<` para un crescendo (se abre) o `>` para un diminuendo (se cierra).

    **Desde la paleta:**
    1. Seleccionar el rango.
    2. Hacer clic en el regulador deseado en la paleta **Dinámicas**.


    ### Reguladores con dinámicas en los extremos

    La forma más común y correcta de usar reguladores es acompañarlos con dinámicas:
    - Escribir ***p*** en la nota donde comienza el crescendo.
    - Seleccionar desde esa nota hasta la nota donde termina.
    - Presionar `<`.
    - Escribir ***f*** en la nota final del regulador.

    MuseScore alinea automáticamente el regulador con las dinámicas de los extremos si comparten la misma asignación de voz y posición.

    ### Altura y ángulo del regulador

    - **Altura**: seleccionar el regulador, luego arrastrar el tirador inferior de la apertura hacia arriba o abajo, o usar las teclas `↑` / `↓`.
    - **Ángulo**: en el panel **Propiedades**, activar **Permitir diagonal**. Luego se pueden mover independientemente los extremos del regulador en el plano vertical.

    ### Opciones avanzadas

    - **Círculo de *niente***: en el panel Propiedades, activar "Niente circle" para dibujar un pequeño círculo en la punta del regulador, indicando que el sonido viene de la nada o se desvanece a la nada.
    - ***Cresc. / dim.* con línea de texto**: para pasajes largos donde un regulador tradicional sería demasiado extenso, usar las líneas *cresc.* o *dim.* de la paleta **Dinámicas**. Funcionan igual que los reguladores pero se dibujan como texto seguido de una línea punteada.

???+ note "Tempo: marcas metronómicas, palabras y cambios graduales"

    El tempo controla la **velocidad** de la música. MuseScore reproduce automáticamente las marcas de tempo que coloques en la partitura.

    ### Tipos de marcas de tempo

    | Tipo | Ejemplo | Cómo se ve | Cómo se usa |
    |---|---|---|---|
    | Marca metronómica | ♩ = 120 | Figura + número | Tempo exacto en pulsos por minuto |
    | Indicación verbal | Allegro, Andante | Palabra en italiano | Tempo aproximado, interpretativo |
    | Combinada | Allegro ♩ = 132 | Palabra + marca | Lo más común en partituras modernas |
    | Modulación métrica | ♩ = ♩. | Dos figuras conectadas | Indica equivalencia entre pulsos al cambiar de compás |

    ### Agregar una marca de tempo

    1. Seleccionar una nota o compás donde debe comenzar el tempo.
    2. Ir a la paleta **Tempo**.
    3. Hacer clic en la marca deseada (ej. "Allegro ♩ = 120").
    4. Para crear una marca metronómica rápida basada en el compás actual: `Alt + Shift + T`.

    ### Editar una marca de tempo

    Hacer doble clic en la marca para entrar en modo de edición. Se puede:
    - Cambiar el texto (ej. de "Allegro" a "Moderato").
    - Cambiar la figura usando la ventana de **Símbolos especiales** (`Shift + F2`).
    - Ajustar el número de BPM.


    ### Cambios graduales de tempo

    La paleta **Tempo** incluye líneas de cambio gradual:
    - **accel.**: accelerando (aumenta velocidad progresivamente). Por defecto, acelera hasta el 133% del tempo original.
    - **rit.**: ritardando (disminuye velocidad). Por defecto, desacelera hasta el 75% del tempo original.
    - **rall.**: rallentando (similar a ritardando, mismo comportamiento por defecto).

    Para aplicarlas: seleccionar el rango de compases sobre el cual debe ocurrir el cambio y hacer clic en la línea deseada.

    En el panel **Propiedades → Reproducción**, se puede ajustar:
    - **Cantidad**: porcentaje del tempo original al llegar al final de la línea.
    - **Método de transición**: Normal (lineal), Ease in (lento al inicio, rápido al final), Ease out (rápido al inicio, lento al final).

    ### Velocidad de reproducción general

    El botón de **Velocidad de reproducción** en la barra de reproducción permite cambiar temporalmente la velocidad de TODA la partitura sin modificar las marcas de tempo escritas. Es un porcentaje del tempo escrito: útil para practicar pasajes difíciles más lento sin cambiar la partitura.

???+ note "Mixer y controles de reproducción"

    MuseScore incluye un mezclador completo y una barra de reproducción que permiten controlar cómo suena cada aspecto de la partitura.

    ### Abrir el Mixer

    - Clic en el botón **Mixer** de la barra de herramientas de ingreso de notas.
    - Menú **Ver → Mixer**.
    - Atajo: `F10`.

    ### Canales del Mixer

    El mixer se organiza en tiras de canal codificadas por color:

    | Color | Canal | Función |
    |---|---|---|
    | Azul | **Instrumento** | Un canal por cada instrumento del score. Controla el sonido, efectos, paneo y volumen de ese instrumento. |
    | Azul | **Metrónomo** | Silenciar/activar el metrónomo y cambiar su sonido y volumen. |
    | Verde | **Aux 1 / Aux 2** | Canales auxiliares para efectos compartidos. Aux 1 contiene Muse Reverb por defecto. |
    | Rosa | **Master** | Controla el volumen general de toda la partitura. |

    ### Controles por canal (de arriba hacia abajo)

    1. **Sound (Sonido)**: el instrumento virtual asignado. Se puede cambiar sin afectar la notación del pentagrama: pasar el ratón sobre el nombre → clic en el desplegable → elegir otro sonido.
    2. **Audio FX**: efectos VST o Muse Reverb. Clic en una ranura vacía → elegir efecto. Se procesan de arriba hacia abajo.
    3. **Aux sends**: cuánto del efecto del canal auxiliar se aplica a este instrumento. La primera fila (Reverb) controla la reverberación.
    4. **Pan**: control giratorio para mover el sonido a la izquierda o derecha en el campo estéreo.
    5. **Volume (Volumen)**: deslizador para ajustar el volumen del canal.
    6. **Mute / Solo**: Mute silencia el canal; Solo silencia todos los demás.


    ### Cambio de sonido a mitad de la partitura

    Para que un mismo pentagrama suene con diferentes instrumentos en distintas secciones:
    1. Seleccionar la nota o compás donde debe cambiar el sonido.
    2. Ir a **Añadir → Texto → Cambio de instrumento** (o desde la paleta **Texto**).
    3. Elegir el nuevo instrumento.
    4. El pentagrama mantiene su notación original pero el Mixer crea un nuevo canal para el sonido cambiado.

    Esto es especialmente útil en partituras de teatro musical o arreglos donde un instrumentista toca múltiples instrumentos (ej. flauta y flautín, clarinete y clarinete bajo).

    ### Barra de reproducción

    Los controles básicos, de izquierda a derecha:

    | Botón | Función | Atajo |
    |---|---|---|
    | **Rewind** | Ir al inicio del score (o del loop) | — |
    | **Play / Pause** | Iniciar o pausar la reproducción | `Espacio` |
    | **Toggle loop** | Activar repetición en bucle de una selección | — |
    | **Metrónomo** | Activar/desactivar clic del metrónomo | — |
    | **Playback settings** | Opciones avanzadas: entrada MIDI, repetir compases, acordes, etc. | — |
    | **Contadores** | Muestra posición en tiempo (mm:ss) y en compases:pulsos | — |
    | **Velocidad** | Control deslizante para cambiar velocidad de reproducción | — |

    ### Ajustes de reproducción útiles

    Desde **Playback settings** (rueda dentada):
    - **Play repeats**: reproduce repeticiones (saltos, casillas). Desactivar para escuchar la estructura sin repeticiones.
    - **Play chord symbols**: reproduce los símbolos de acorde como armonía de acompañamiento.
    - **Pan score automatically**: desplaza la vista de la partitura automáticamente durante la reproducción.
    - **Hear playback when editing**: previsualiza el sonido de cada nota al seleccionarla o editarla.

    !!! tip "El Mixer no modifica la partitura, solo el audio"
        Cambiar un sonido en el Mixer no altera la notación del pentagrama ni la transposición. Si querés que el pentagrama refleje el cambio (clave, armadura, transposición), usá **Cambio de instrumento** desde la paleta Texto. Si solo querés escuchar otro timbre sin tocar la notación, usá el Mixer.

---

## Actividad en Classroom

### Tarea: S10 — Dinámicas, tempo y reproducción

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S10_dinamicas.mscz`, una partitura para cuarteto de cuerdas (violín I, violín II, viola, violonchelo) en Do mayor, 4/4, 32 compases con una pieza breve sin dinámicas ni marcas de tempo; (b) `ejercicio_S10_mixer.mscz`, una partitura para instrumento solista (flauta) con cambios de sonido sugeridos.

1. **Agregar dinámicas a cada instrumento.** Abrí `ejercicio_S10_dinamicas.mscz`:
    - En cada pentagrama, agregá al menos 4 dinámicas diferentes distribuidas a lo largo de los 32 compases. Usá la paleta **Dinámicas** o el popup (`Ctrl + D`).
    - Asegurate de que las dinámicas tengan sentido musical: una frase que comienza suave puede crecer hacia un clímax y luego disminuir.
    - Experimentá con dinámicas extremas (***pp*** y ***ff***) para notar el contraste.

2. **Insertar reguladores.** En los mismos pentagramas:
    - Colocá al menos 3 reguladores: 2 de crescendo (`<`) y 1 de diminuendo (`>`).
    - Cada regulador debe estar acompañado de una dinámica en su inicio y otra en su final (ej. ***p*** `<` ***f***).
    - Ajustá la altura de al menos un regulador arrastrando su tirador.
    - Probá un regulador con círculo de *niente* (desde el panel Propiedades) en el violonchelo: que comience desde el silencio.

3. **Marcas de tempo.** Sobre el pentagrama del violín I:
    - Insertá una marca de tempo al inicio: "Allegro ♩ = 120".
    - En el compás 17, insertá un cambio de tempo: "Adagio ♩ = 60".
    - Entre los compases 24 y 28, insertá una línea de **ritardando** (rit.) desde la paleta **Tempo**.
    - En el compás 29, insertá "a tempo" para recuperar la velocidad original.
    - Reproducí y escuchá los cambios de velocidad.

4. **Exploración del Mixer.** Abrí `ejercicio_S10_mixer.mscz`. El archivo contiene una melodía para flauta en Do mayor, 4/4, 16 compases. Abrí el Mixer (`F10`) y realizá lo siguiente:
    - Cambiá el sonido de la flauta por un oboe en los compases 1–8 (sin modificar la notación).
    - Cambiá el sonido a un clarinete en los compases 9–16 usando **Añadir → Texto → Cambio de instrumento**. Observá cómo se crea un nuevo canal en el Mixer.
    - Ajustá el paneo del oboe ligeramente a la izquierda y el del clarinete ligeramente a la derecha.
    - Activá el metrónomo durante la reproducción y escuchá la pieza con los cambios.
    - Experimentá con el control de velocidad de reproducción: escuchá la pieza al 50%, al 100% y al 150%.

5. **Documentación de la experiencia.** Elaborá un breve informe (media página) donde expliques:
    - ¿Cómo afectaron las dinámicas y los reguladores a la expresión de la pieza del cuarteto?
    - ¿Qué diferencias notaste entre cambiar el sonido desde el Mixer y cambiarlo con "Cambio de instrumento"?
    - ¿Para qué situaciones usarías cada método de cambio de sonido?

### Entregables

- [ ] `APELLIDO_Nombre_S10_dinamicas_v01.mscz` (cuarteto con dinámicas, reguladores y marcas de tempo)
- [ ] `APELLIDO_Nombre_S10_dinamicas_v01.pdf`
- [ ] `APELLIDO_Nombre_S10_mixer_v01.mscz` (flauta con cambios de sonido)
- [ ] `APELLIDO_Nombre_S10_mixer_v01.pdf`
- [ ] Captura del Mixer mostrando los canales con los cambios aplicados
- [ ] Informe de la experiencia (media página, PDF o Google Docs)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Dinámicas | ≥4 dinámicas diferentes por pentagrama; distribución coherente con la frase musical | 2–3 dinámicas por pentagrama o distribución poco musical | Sin dinámicas o mal distribuidas |
| Reguladores | ≥2 crescendo y ≥1 diminuendo; cada uno acompañado de dinámicas en los extremos | Reguladores presentes pero sin dinámicas de referencia | Sin reguladores |
| Marcas de tempo | Tempo inicial, cambio en c.17, ritardando y "a tempo" correctamente insertados y audibles | 2–3 marcas presentes | ≤1 marca de tempo |
| Mixer | Sonidos cambiados con ambos métodos; paneo ajustado; metrónomo usado | Solo un método de cambio usado | Sin cambios en el Mixer |
| Informe | Explica los 3 puntos con claridad; usa ejemplos del ejercicio | Explica 2 de 3 puntos | No entregó el informe |

---

*Basado en: MuseScore Studio 4 Handbook — Dynamics and hairpins, Tempo markings, Mixer, Playback controls | https://handbook.musescore.org*
