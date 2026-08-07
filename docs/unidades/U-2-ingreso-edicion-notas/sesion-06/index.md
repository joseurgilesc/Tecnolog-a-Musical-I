# Sesión 6: Compases, métrica y operaciones de compás

📚 Handbook → Notation: Rhytm, meter & measures — Time signatures, Measure operations, Barlines, Measure numbering, Pickup & non-metered measures | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consulta esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="compas"></a> **Compás (measure)** | Unidad métrica que agrupa pulsos según la indicación de compás. Se delimita visualmente por líneas divisorias y su contenido rítmico debe sumar exactamente lo que indica la fracción de compás. |
    | <a id="indicacion-compas"></a> **Indicación de compás (time signature)** | Fracción escrita al inicio de la partitura (y en cada cambio métrico) donde el numerador indica cuántos pulsos entran en el compás y el denominador qué figura equivale a un pulso. Ejemplo: 4/4 = cuatro pulsos de negra. |
    | <a id="compas-simple"></a> **Compás simple** | Compás cuyo pulso se divide naturalmente en mitades. Los más comunes: 2/4 (binario), 3/4 (ternario) y 4/4 (cuaternario). |
    | <a id="compas-compuesto"></a> **Compás compuesto** | Compás cuyo pulso se divide naturalmente en tercios. Se reconoce porque el numerador es múltiplo de 3: 6/8, 9/8, 12/8. En 6/8 hay dos pulsos, cada uno dividido en tres corcheas. |
    | <a id="anacrusa"></a> **Anacrusa / Compás de pickup** | Compás inicial incompleto que comienza en un pulso débil. Su duración se descuenta del último compás de la pieza (o de la sección). La numeración de compases arranca en el primer compás completo. |
    | <a id="barra-divisoria"></a> **Barra divisoria / Línea divisoria (barline)** | Línea vertical que separa compases. Las variantes más usadas son: barra simple (separación normal), barra doble (cambio de sección métrica o armadura) y barra final (doble con una línea gruesa). |
    | <a id="insertar-compas"></a> **Insertar compás** | Agregar uno o más compases vacíos en una posición específica, desplazando el contenido posterior hacia adelante. Atajo: `Ins` para uno, `Ctrl + Ins` para varios. |
    | <a id="eliminar-compas"></a> **Eliminar compás** | Suprimir compases completos con todo su contenido. Atajo: `Ctrl + Supr` (`Cmd + Supr` en macOS). No debe confundirse con `Supr`, que borra las notas pero conserva el compás lleno de silencios. |
    | <a id="numeracion-compases"></a> **Numeración de compases** | Números que identifican cada compás. MuseScore los genera automáticamente. Pueden ocultarse, mostrarse en cada sistema, excluir compases del conteo y reiniciar la numeración después de un salto de sección. |

???+ note "Operaciones de compás: añadir, insertar, eliminar, duplicar"

    Dominar las operaciones de compás es esencial para estructurar tu partitura. Cada operación tiene un efecto distinto y usarlas correctamente evita tener que reescribir secciones enteras.

    ### Añadir compases al final

    | Método | Acción |
    |---|---|
    | Un compás al final | `Ctrl + B` (`Cmd + B` en macOS) |
    | Varios compases al final | `Alt + Shift + B` → ingresar cantidad |
    | Menú | **Añadir → Compases → Al final de la partitura** |

    Los compases se añaden justo después del último compás existente, con el mismo tipo de barra divisoria.

    ### Insertar compases en el medio

    Insertar desplaza todo el contenido desde ese punto hacia adelante, abriendo espacio donde lo necesitas.

    | Método | Acción |
    |---|---|
    | Un compás antes de la selección | Seleccionar un compás → `Ins` |
    | Varios compases antes | Seleccionar → `Ctrl + Ins` (`Cmd + Ins`) → ingresar cantidad |
    | Menú contextual | Clic derecho en compás → **Insertar compases** → elegir ubicación y cantidad |


    ### Eliminar compases

    | Operación | Atajo | Resultado |
    |---|---|---|
    | **Eliminar compás** completo | `Ctrl + Supr` (`Cmd + Supr`) | El compás desaparece; los siguientes se desplazan hacia atrás |
    | **Borrar contenido** (vaciar compás) | `Supr` | Las notas se borran pero el compás permanece lleno de silencios |
    | **Eliminar rango seleccionado** | **Herramientas → Eliminar rango seleccionado** | Elimina los compases del rango |

    !!! warning "La diferencia entre `Supr` y `Ctrl + Supr`"
        Este es uno de los errores más frecuentes al empezar. `Supr` limpia el interior del compás pero el compás sigue ahí. `Ctrl + Supr` lo elimina por completo. Si tu partitura tiene un compás de más que interrumpe la estructura, usa `Ctrl + Supr`, no `Supr`.

    ### Duplicar compases

    | Método | Acción |
    |---|---|
    | Copiar y pegar | Seleccionar compás → `Ctrl + C` → seleccionar destino → `Ctrl + V` |
    | Repetir (`R`) | Seleccionar compás(es) → `R` (pega justo después) |

    La tecla `R` es particularmente útil para secciones con patrones repetitivos. Si seleccionas 2 compases y presionas `R`, los duplica inmediatamente a continuación.

    ### Insertar vs. Añadir: resumen visual

    | Operación | ¿Dónde? | ¿Desplaza el contenido existente? |
    |---|---|---|
    | `Ctrl + B` | Al final | No (no hay nada después) |
    | `Ins` | En el medio | Sí, todo se mueve a la derecha |
    | `Ctrl + Ins` | En el medio (varios) | Sí |
    | `Ctrl + Supr` | Cualquiera | Los compases siguientes se mueven a la izquierda |

???+ note "Indicaciones de compás: simples y compuestos"

    La indicación de compás define la estructura métrica de la partitura. MuseScore la aplica desde la paleta **Indicaciones de compás** (Time signatures).

    ### Agregar o cambiar una indicación de compás

    1. Seleccionar un compás, nota o silencio donde quieres que comience el cambio.
    2. Hacer clic en la indicación deseada de la paleta **Indicaciones de compás**.

    Alternativamente, arrastrar la indicación desde la paleta hasta el compás.

    !!! important "El cambio de compás ocurre al inicio del compás"
        Actualmente, los cambios de compás solo pueden ocurrir al principio de un compás. Al cambiar la métrica, MuseScore re-agrupa automáticamente los compases siguientes, por lo que conviene revisar que ningún material musical se haya perdido en el proceso.

    ### Compases simples más usados

    | Compás | Tipo | Pulsos | Subdivisión del pulso |
    |---|---|---|---|
    | 2/4 | Binario simple | 2 negras | 4 corcheas (2+2) |
    | 3/4 | Ternario simple | 3 negras | 6 corcheas (2+2+2) |
    | 4/4 | Cuaternario simple | 4 negras | 8 corcheas (2+2+2+2) |
    | 2/2 (₵) | Binario simple (alla breve) | 2 blancas | 4 negras (2+2) |

    ### Compases compuestos más usados

    | Compás | Tipo | Pulsos | Subdivisión del pulso |
    |---|---|---|---|
    | 6/8 | Binario compuesto | 2 negras con puntillo | 6 corcheas (3+3) |
    | 9/8 | Ternario compuesto | 3 negras con puntillo | 9 corcheas (3+3+3) |
    | 12/8 | Cuaternario compuesto | 4 negras con puntillo | 12 corcheas (3+3+3+3) |

    !!! tip "Cómo distinguir simple de compuesto"
        En un compás simple, el numerador suele ser 2, 3 o 4. En un compás compuesto, el numerador es múltiplo de 3 (6, 9, 12) y el denominador suele ser 8. La diferencia práctica: en 6/8 sientes **dos** pulsos (no seis) y cada pulso se subdivide en tres.

    ### Crear una indicación de compás personalizada

    Si necesitas un compás que no está en la paleta (ej. 5/4, 7/8):

    1. En la paleta **Indicaciones de compás**, hacer clic en **Más**.
    2. Clic en **Crear indicación de compás**.
    3. Ingresar numerador y denominador en **Valor**.
    4. Si quieres que se vea distinto (ej. "3+2/4"), escríbelo en **Texto**.
    5. Clic en **Añadir** para guardarlo en la paleta.

    ### Cambios de compás dentro de una obra

    MuseScore permite cambiar la métrica en cualquier punto de la partitura. Para hacerlo:
    1. Seleccionar el compás donde debe comenzar el nuevo compás.
    2. Elegir la nueva indicación en la paleta.
    3. Revisar que las barras de compás siguientes no hayan quedado con material desplazado.


    ### Compases de cortesía (courtesy time signatures)

    Cuando un cambio de compás coincide con el inicio de un sistema, MuseScore muestra automáticamente una indicación de cortesía al final del sistema anterior (entre paréntesis). Esto se puede desactivar desde **Formato → Estilo → Claves, armaduras e indicaciones de compás**.

???+ note "Anacrusa y compases incompletos"

    ### ¿Qué es una anacrusa?

    Una anacrusa (pickup measure) es un compás inicial que no está completo: empieza en un pulso débil. La duración que falta se descuenta del último compás de la pieza o sección. Por convención, la numeración de compases comienza en el primer compás **completo** (el compás 1 nunca es la anacrusa).

    ### Crear una anacrusa al iniciar la partitura

    Al crear una partitura nueva, en la segunda página del asistente:
    1. Clic en **Compases**.
    2. Marcar **Crear anacrusa**.
    3. Elegir la duración del pickup (ej. una corchea en 4/4).

    ### Convertir un compás existente en anacrusa

    1. Clic derecho en el compás → **Propiedades del compás**.
    2. En **Duración del compás**, junto a **Real**, ajustar el numerador y denominador.
    3. Clic en **Aceptar**. El compás se acorta.

    ### Compases con duración irregular

    Para crear compases que duran más o menos que la indicación de compás (ej. un compás de 5/4 en una partitura en 4/4):
    1. Clic derecho en el compás → **Propiedades del compás**.
    2. Modificar los valores de **Real**.
    3. Se mostrará un pequeño `+` o `−` sobre el compás como advertencia visual.

    !!! info "¿Para qué sirve un compás irregular?"
        Casos típicos: compases de cadenza, compases finales que completan la anacrusa inicial, o pasajes con métrica libre donde no conviene cambiar la indicación de compás para un solo compás.

???+ note "Líneas divisorias: simples, dobles, finales"

    Las barras de compás se aplican desde la paleta **Líneas divisorias** (Barlines).

    ### Tipos de barras y cuándo usarlas

    | Barra | Uso musical |
    |---|---|
    | **Simple** | Separación normal entre compases. Es la que usa MuseScore por defecto. |
    | **Doble** | Cambio de sección, cambio de armadura, cambio de compás, o antes de un cambio de tempo importante. |
    | **Final** | Fin de la partitura o de un movimiento. Tiene una línea fina seguida de una gruesa. |
    | **Repetición inicial** | Indica dónde comienza una sección que se repite (dos puntos mirando hacia la derecha). |
    | **Repetición final** | Indica dónde termina una sección que se repite (dos puntos mirando hacia la izquierda). |
    | **Punteada** | Uso editorial: divide compases muy largos o indica sub-agrupaciones métricas. |

    ### Cambiar el tipo de barra

    **Para toda la partitura** (todas las voces):
    1. Seleccionar una o más barras en cualquier pentagrama.
    2. Hacer clic en la barra deseada en la paleta.

    **Para un solo pentagrama** (barra local):
    1. Seleccionar la barra.
    2. Mantener `Ctrl` (`Cmd` en macOS) y hacer clic en la barra deseada de la paleta.

    ### Insertar una barra a mitad del compás

    1. Seleccionar una nota o silencio.
    2. Hacer clic en una barra de la paleta.

    Esto agrega una barra **visual** después de la nota seleccionada, sin dividir realmente el compás. Para dividir un compás en dos (con barras reales), usar **Herramientas → Compases → Dividir compás antes de la nota/silencio seleccionado**.


???+ note "Numeración de compases"

    MuseScore numera los compases automáticamente. Por defecto, muestra el número al inicio de cada sistema (excepto el primero).

    ### Configurar la numeración para todo el score

    1. Ir a **Formato → Estilo → Numeración de compases**.
    2. Activar **Mostrar numeración de compases**.
    3. Elegir la frecuencia: al inicio de cada sistema, cada X compases, o cada compás.

    ### Excluir un compás del conteo

    1. Clic derecho en el compás → **Propiedades del compás**.
    2. Marcar **Excluir del conteo de compases**.

    Esto se aplica automáticamente a las anacrusas creadas con el asistente.

    ### Modificar el número de un compás

    1. Clic derecho en el compás → **Propiedades del compás**.
    2. En **Agregar al número de compás**, ingresar un valor positivo o negativo.

    Útil cuando un score tiene varios movimientos: si el primer movimiento ocupa 80 compases, configurar `−80` en el primer compás del segundo movimiento lo hará comenzar en 1.

    ### Reiniciar numeración con saltos de sección

    Por defecto, un **salto de sección** reinicia la numeración. Para desactivarlo:
    1. Seleccionar el salto de sección.
    2. En el panel **Propiedades**, desmarcar **Reiniciar numeración de compases en nueva sección**.

---

## 🎹 Desafío de Shortcuts — Sesión 6

Practica los atajos de métrica y operaciones de compás. Al final verás tus errores para repasarlos en MuseScore.

[🎮 Jugar Desafío S6](../../juegos/shortcuts-game.html?sesion=6){ .md-button .md-button--primary }

---

Ver el ejercicio en Classroom.

---

*Basado en: MuseScore Studio 4 Handbook — Time signatures, Barlines, Measure properties, Measure numbering, Pickup and non-metered measures; MuseScore 3 Handbook — Notation: Time signatures, Measure operations, Barlines, Measure rests, Measure numbering | https://handbook.musescore.org*
