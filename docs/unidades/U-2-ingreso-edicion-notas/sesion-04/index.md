# Sesión 4: Ingreso de notas

📚 Handbook → Basics: Entering notes and rests, Alternative note input methods, Editing notes and rests | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="modo-ingreso"></a> **Modo de ingreso de notas** | Estado de MuseScore en el que cada tecla o clic produce una nota en la partitura. Se activa con la tecla `N` o con el ícono del lápiz ✏️ en la barra de herramientas. El cursor azul indica dónde se insertará la siguiente nota. |
    | <a id="valor-ritmico"></a> **Valor rítmico / Duración** | La figura que determina cuánto dura una nota: redonda (1), blanca (2), negra (3), corchea (4), semicorchea (5), fusa (6), semifusa (7). Los números entre paréntesis son los atajos de teclado. |
    | <a id="puntillo"></a> **Puntillo** | Punto colocado a la derecha de una figura que aumenta su duración en la mitad de su valor original. Se ingresa con la tecla `.` (punto) después de seleccionar la duración. |
    | <a id="alteracion"></a> **Alteración** | Signo que modifica la altura de una nota: sostenido (♯), bemol (♭) o becuadro (♮). Se ingresa con `+` (sostenido), `-` (bemol) o `=` (becuadro) antes de la nota. |
    | <a id="ligadura-prolongacion"></a> **Ligadura de prolongación** | Línea curva que une dos notas del mismo sonido para sumar sus duraciones. Se ingresa con la tecla `T` después de la primera nota. No debe confundirse con la ligadura de fraseo. |
    | <a id="silencio"></a> **Silencio** | Signo que indica ausencia de sonido durante una duración determinada. En modo de ingreso, se introduce con la tecla `0` (cero) después de seleccionar la duración. |
    | <a id="acorde"></a> **Acorde** | Combinación de dos o más notas que suenan simultáneamente y comparten la misma plica. Se construye manteniendo `Shift` mientras se ingresan las notas adicionales con el teclado. |
    | <a id="octava"></a> **Octava** | Distancia entre dos notas del mismo nombre separadas por ocho grados. En el ingreso, `Ctrl + ↑` sube la nota una octava y `Ctrl + ↓` la baja (`Cmd` en macOS). |
    | <a id="cursor-ingreso"></a> **Cursor de ingreso** | Indicador visual (línea azul vertical) que muestra la posición donde se insertará la siguiente nota dentro del compás. Avanza automáticamente con cada nota ingresada. |
    | <a id="modo-normal"></a> **Modo normal** | Estado por defecto de MuseScore cuando no se está ingresando notas. Se sale del modo de ingreso con `Esc` o `N`. En modo normal se realizan operaciones de edición, selección y formato. |

???+ note "El modo de ingreso de notas: la puerta de entrada"

    Todo lo que escribas en MuseScore —una melodía, un acorde, un ritmo de percusión— comienza por activar el **modo de ingreso de notas**. Este modo convierte tu teclado y ratón en herramientas de escritura musical.

    ![Ingreso de notas con teclado](https://handbook.musescore.org/~gitbook/image?url=https%3A%2F%2F3455969201-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FP81HaeapLzzJGtG6DSwH%252Fuploads%252Fgit-blob-9d5afedf062319a4212627db63153790aeeda18d%252Fentering-notes.gif%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=7968d0e&sv=2)

    ### Activar y desactivar el modo de ingreso

    | Acción | Atajo / Método |
    |---|---|
    | **Entrar** al modo de ingreso | Tecla `N` o clic en el ícono del lápiz ✏️ en la barra de herramientas |
    | **Salir** del modo de ingreso | Tecla `N` de nuevo o tecla `Esc` |
    | Indicador visual | Aparece un cursor azul en el compás donde se insertará la siguiente nota |

    Una vez activado, **el orden de operaciones es siempre el mismo**:

    1. Seleccioná la **duración** (valor rítmico) que querés escribir.
    2. Indicá la **altura** (nombre de la nota, con o sin alteración).


    ### Seleccionar la duración

    Los valores rítmicos se seleccionan de dos maneras:

    | Método | Acción |
    |---|---|
    | **Ratón** | Clic en el ícono de la figura en la barra de herramientas de ingreso |
    | **Teclado** | Teclas `1` a `9`: 1 = semifusa, 2 = fusa, 3 = semicorchea, 4 = corchea, 5 = negra, 6 = blanca, 7 = redonda, 8 = longa, 9 = breve |

    ![Cambio de duraciones rítmicas](https://handbook.musescore.org/~gitbook/image?url=https%3A%2F%2F3455969201-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FP81HaeapLzzJGtG6DSwH%252Fuploads%252Fgit-blob-4c5bc450dcf699f7f17c0e9116be1486109e207e%252Fchaning-note-durations.gif%3Falt%3Dmedia&width=768&dpr=2&quality=100&sign=ba468662&sv=2)

    Las teclas `4`, `5` y `6` (corchea, negra, blanca) están en el centro del teclado numérico y corresponden a los valores más usados. Las figuras más cortas usan números más bajos; las más largas, números más altos.

    !!! tip "Pensá la duración primero, la altura después"
        El error más frecuente al empezar es querer escribir la nota directamente. En MuseScore **primero se elige cuánto dura** y después **qué nota es**. Si invertís el orden, el programa no va a interpretar lo que esperás.

    ### Salir del modo de ingreso

    Salir del modo de ingreso (`Esc` o `N`) es necesario para:
    - Seleccionar elementos ya escritos.
    - Copiar, pegar, eliminar secciones.
    - Agregar dinámicas, textos, articulaciones.
    - Cambiar propiedades de la partitura.

    Mientras estés en modo de ingreso, casi todo lo que hagas insertará notas. El modo normal es tu espacio de edición.

???+ note "Ingreso con teclado vs. ingreso con ratón: dos caminos, un destino"

    MuseScore ofrece dos métodos principales para ingresar notas. Ninguno es mejor en absoluto: cada uno brilla en situaciones distintas.

    ### Ingreso con teclado de computador

    Es el método más rápido para la mayoría de los usuarios una vez que se memorizan las teclas.

    | Paso | Acción |
    |---|---|
    | 1 | Activá el modo de ingreso (`N`) |
    | 2 | Seleccioná la duración (`1`–`9`) |
    | 3 | Presioná la letra de la nota (`A`–`G`) |
    | 4 | Opcional: aplicá alteración antes (`+`, `-`, `=`) |

    **Ejemplo**: para escribir un Fa♯ negra, la secuencia es: `N` → `5` → `+` → `F`.

    MuseScore elige automáticamente la octava más cercana a la nota anterior. Si necesitás cambiar la octava:

    | Acción | Atajo |
    |---|---|
    | Subir una octava | `Ctrl + ↑` (`Cmd + ↑` en macOS) |
    | Bajar una octava | `Ctrl + ↓` (`Cmd + ↓` en macOS) |


    ### Ingreso con ratón

    El ratón permite ver físicamente dónde caerá la nota antes de insertarla.

    | Paso | Acción |
    |---|---|
    | 1 | Activá el modo de ingreso (`N`) |
    | 2 | Seleccioná la duración en la barra de herramientas |
    | 3 | Posicioná el cursor sobre la línea o espacio deseado (aparece una previsualización de la nota) |
    | 4 | Hacé clic para insertar la nota |

    **Ventaja**: no necesitás memorizar las letras de las notas ni las teclas de duración. **Limitación**: es más lento que el teclado en pasajes largos y puede ser impreciso en notas muy agudas o graves (MuseScore podría interpretar el clic como dirigido al pentagrama vecino).


    ### Comparación

    | Situación | ¿Teclado o ratón? |
    |---|---|
    | Melodía larga con muchas notas | **Teclado**: mucho más rápido una vez dominado |
    | Acordes complejos con alteraciones | **Teclado**: `Shift` + letras es más preciso |
    | Primeros ejercicios, estás aprendiendo | **Ratón**: la previsualización ayuda a entender dónde cae cada nota |
    | Notas muy agudas o graves fuera del pentagrama | **Teclado** + ajuste de octava |
    | Editar una nota suelta ya escrita | **Ratón**: clic directo sobre lo que querés cambiar |

???+ note "Valores rítmicos, puntillos y silencios"

    ### Valores rítmicos: del más largo al más corto

    | Figura | Nombre | Atajo | ¿Cuántas entran en un 4/4? |
    |---|---|---|---|
    | 𝅝 | Redonda | `7` | 1 |
    | 𝅗𝅥 | Blanca | `6` | 2 |
    | 𝅘𝅥 | Negra | `5` | 4 |
    | 𝅘𝅥𝅮 | Corchea | `4` | 8 |
    | 𝅘𝅥𝅯 | Semicorchea | `3` | 16 |
    | 𝅘𝅥𝅰 | Fusa | `2` | 32 |
    | 𝅘𝅥𝅱 | Semifusa | `1` | 64 |

    La duración seleccionada permanece activa hasta que elijas otra. Si escribiste una negra y la siguiente nota también es negra, no necesitás volver a presionar `5`: MuseScore mantiene la última duración.

    ### Puntillo

    El puntillo (`.`) aumenta la duración de una figura en la mitad de su valor:
    - Negra con puntillo = negra + corchea (1.5 tiempos en 4/4)
    - Blanca con puntillo = blanca + negra (3 tiempos en 4/4)

    Para ingresarlo: presioná `.` **después** de seleccionar la duración y **antes** de ingresar la nota. Ejemplo: `N` → `5` → `.` → `C` produce un Do negra con puntillo.

    El puntillo se puede aplicar a silencios de la misma manera.

    ### Silencios

    Cada valor rítmico tiene su silencio correspondiente. Se ingresa con la tecla `0` (cero) en lugar de una letra de nota:

    | Secuencia | Resultado |
    |---|---|
    | `N` → `5` → `0` | Silencio de negra |
    | `N` → `4` → `0` | Silencio de corchea |
    | `N` → `4` → `.` → `0` | Silencio de corchea con puntillo |

    También podés hacer clic derecho en el pentagrama (en modo ingreso) o usar el botón de silencio en la barra de herramientas.


    !!! info "Los silencios no son opcionales"
        En MuseScore, cada compás debe estar rítmicamente completo. Si dejás pulsos vacíos sin escribir silencios, MuseScore los mostrará automáticamente como silencios grises (no imprimibles) o generará un compás incompleto. Acostumbrate a escribir TODOS los silencios desde el principio.

???+ note "Alteraciones, acordes y ligaduras de prolongación"

    ### Alteraciones

    Las alteraciones se aplican a la nota que vas a ingresar. La secuencia es: **seleccionar duración → aplicar alteración → ingresar nota**.

    | Alteración | Tecla | Símbolo |
    |---|---|---|
    | Sostenido | `+` | ♯ |
    | Bemol | `-` | ♭ |
    | Becuadro | `=` | ♮ |

    También podés usar los botones de la barra de herramientas de ingreso.

    **Regla importante**: si escribís un Fa♯ en un compás, todos los Fa siguientes dentro del MISMO compás serán Fa♯ aunque no lleven el signo escrito. MuseScore aplica esta convención de notación automáticamente. Al cambiar de compás, la alteración se cancela (salvo que la armadura la incluya).

    Para cambiar una alteración después de ingresada: seleccioná la nota y usá `↑` (sube un semitono, escribe con sostenidos) o `↓` (baja un semitono, escribe con bemoles).

    ### Acordes

    Un acorde se construye agregando notas sobre una nota base. La primera nota se ingresa normalmente; las siguientes se añaden con `Shift`:

    | Paso | Acción |
    |---|---|
    | 1 | `N` → `5` → `C` (Do negra, nota base) |
    | 2 | `Shift + E` (añade Mi sobre el Do) |
    | 3 | `Shift + G` (añade Sol sobre el Mi) |
    | Resultado | Acorde de Do mayor en negra |

    !!! tip "Construí los acordes desde abajo hacia arriba"
        MuseScore añade las notas hacia arriba desde la nota base. Por eso conviene ingresar primero la nota más grave del acorde y luego ir agregando las más agudas con `Shift`. Si empezás por la nota aguda, tendrías que usar `Ctrl + ↓` para bajar las siguientes.

    También podés ingresar acordes con el ratón (clic en las posiciones deseadas) o con teclado MIDI (presionando varias teclas simultáneamente).

    ### Ligaduras de prolongación

    La ligadura de prolongación une dos notas del **mismo sonido** para que suenen como una sola nota continua. Es distinta de la ligadura de fraseo (curva sobre notas diferentes que indica legato).

    Para ingresar una ligadura de prolongación:

    1. Ingresá la primera nota normalmente.
    2. Seleccioná la **duración** de la segunda nota.
    3. Presioná `T` (de *tie*).

    MuseScore crea automáticamente la segunda nota con la misma altura y la ligadura entre ambas.


    !!! warning "No confundas ligadura de prolongación con ligadura de fraseo"
        - **Ligadura de prolongación** (`T`): une dos notas del mismo sonido. Suma duraciones.
        - **Ligadura de fraseo** (paleta "Líneas" o atajo `S`): curva sobre varias notas de diferente altura. Indica articulación legato.
        Si usás una cuando corresponde la otra, la reproducción y la lectura serán incorrectas.

---

## Actividad en Classroom

### Tarea: S04 — Transcripción con ingreso de notas

> **Material necesario**: el docente proporcionará un PDF con una melodía de 16 compases para transcribir. La melodía incluye redondas, blancas, negras, corcheas, semicorcheas, puntillos, alteraciones, ligaduras de prolongación y silencios en compás de 4/4.

1. **Creá una partitura nueva** para el instrumento que indique el docente (flauta, violín u oboe). Configurá la armadura, el compás y el tempo que aparecen en el PDF. La partitura debe tener 16 compases exactos.

2. **Transcribí la melodía** usando **teclado de computador** (letras `A`–`G`). Ingresá:
    - Todas las notas con sus duraciones correctas (redondas, blancas, negras, corcheas, semicorcheas).
    - Todos los silencios donde corresponda (tecla `0`).
    - Todos los puntillos donde aparezcan (tecla `.`).
    - Todas las alteraciones accidentales (teclas `+`, `-`, `=`).
    - Todas las ligaduras de prolongación (tecla `T`).

3. **Construí al menos dos acordes** (de 3 notas cada uno) en los lugares indicados en el PDF, usando `Shift + letra` para añadir notas a la nota base.

4. **Verificá la completitud de los compases**: seleccioná cada compás y revisá que las duraciones sumen exactamente lo que indica la métrica (en 4/4, cada compás debe sumar 4 tiempos).

5. **Reproducí la melodía** y comparala con la referencia del docente. Corregí cualquier nota, ritmo o silencio que no coincida.

6. **Repetí el ejercicio** (en una segunda partitura o en compases adicionales) usando únicamente el **ratón** para ingresar las notas. No uses el teclado para las alturas.

7. **Compará tu experiencia**: escribí un párrafo breve (5–8 líneas) comparando el ingreso con teclado y con ratón. ¿Cuál te resultó más rápido? ¿Más preciso? ¿En qué situaciones usarías cada uno?

### Entregables

- [ ] `APELLIDO_Nombre_S04_Teclado_v01.mscz` (melodía ingresada con teclado)
- [ ] `APELLIDO_Nombre_S04_Teclado_v01.pdf`
- [ ] `APELLIDO_Nombre_S04_Raton_v01.mscz` (melodía ingresada con ratón)
- [ ] `APELLIDO_Nombre_S04_Raton_v01.pdf`
- [ ] Captura de pantalla mostrando el modo de ingreso activo (con el cursor azul visible)
- [ ] Párrafo de comparación teclado vs. ratón

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Alturas | Todas las notas coinciden con el PDF fuente; no hay notas omitidas ni desplazadas | 1–3 errores de altura | ≥4 errores de altura |
| Ritmo y duraciones | Todas las figuras, puntillos y silencios son correctos; cada compás suma lo indicado por la métrica | 1–2 compases con errores rítmicos o incompletos | ≥3 compases con errores de ritmo |
| Alteraciones y ligaduras | Todas las alteraciones accidentales y ligaduras de prolongación están presentes y son correctas | Falta 1 alteración o 1 ligadura | Faltan ≥2 alteraciones o ligaduras |
| Acordes | Los acordes solicitados tienen las 3 notas correctas y se construyeron con el método indicado | Un acorde incompleto o con error | Acordes no realizados |
| Método de ingreso | Ambos archivos reflejan métodos de ingreso distintos (teclado y ratón); la captura muestra el modo de ingreso activo | No es evidente qué método se usó en cada archivo o falta la captura | Solo entregó un archivo o no diferenció los métodos |
| Comparación escrita | El párrafo identifica ventajas y limitaciones concretas de cada método con ejemplos de la experiencia | Comparación vaga sin ejemplos concretos | No entregó la comparación |

---

*Basado en: MuseScore 3 Handbook — Basics: Note input, Note input modes, Edit mode; MuseScore Studio Handbook — Entering notes and rests, Editing notes and rests | https://musescore.org/en/handbook/3*
