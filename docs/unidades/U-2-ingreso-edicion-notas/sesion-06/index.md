# Sesión 6: Compases, métrica y operaciones de compás

📚 Handbook → Notation: Rhytm, meter & measures — Time signatures, Measure operations, Barlines, Measure numbering, Pickup & non-metered measures | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

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

    Insertar desplaza todo el contenido desde ese punto hacia adelante, abriendo espacio donde lo necesitás.

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
        Este es uno de los errores más frecuentes al empezar. `Supr` limpia el interior del compás pero el compás sigue ahí. `Ctrl + Supr` lo elimina por completo. Si tu partitura tiene un compás de más que interrumpe la estructura, usá `Ctrl + Supr`, no `Supr`.

    ### Duplicar compases

    | Método | Acción |
    |---|---|
    | Copiar y pegar | Seleccionar compás → `Ctrl + C` → seleccionar destino → `Ctrl + V` |
    | Repetir (`R`) | Seleccionar compás(es) → `R` (pega justo después) |

    La tecla `R` es particularmente útil para secciones con patrones repetitivos. Si seleccionás 2 compases y presionás `R`, los duplica inmediatamente a continuación.

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

    1. Seleccionar un compás, nota o silencio donde querés que comience el cambio.
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
        En un compás simple, el numerador suele ser 2, 3 o 4. En un compás compuesto, el numerador es múltiplo de 3 (6, 9, 12) y el denominador suele ser 8. La diferencia práctica: en 6/8 sentís **dos** pulsos (no seis) y cada pulso se subdivide en tres.

    ### Crear una indicación de compás personalizada

    Si necesitás un compás que no está en la paleta (ej. 5/4, 7/8):

    1. En la paleta **Indicaciones de compás**, hacer clic en **Más**.
    2. Clic en **Crear indicación de compás**.
    3. Ingresar numerador y denominador en **Valor**.
    4. Si querés que se vea distinto (ej. "3+2/4"), escribilo en **Texto**.
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

## Actividad en Classroom

### Tarea: S06 — Estructura métrica y operaciones de compás

> **Material necesario**: el docente proporcionará el archivo `ejercicio_S06_metrica.mscz` con una partitura para flauta de 24 compases en 4/4 que contiene problemas de estructura métrica.

1. **Auditoría de compases.** Reproducí el archivo `ejercicio_S06_metrica.mscz` y revisá compás por compás:
    - ¿Cada compás suma exactamente 4 tiempos? Identificá los compases que están incompletos o con material sobrante.
    - ¿La música se detiene abruptamente en algún punto? Eso puede indicar un compás eliminado por error.
    - Marcá en una hoja el número de compás y el problema detectado.

2. **Corrección estructural.** Aplicá las operaciones necesarias para que la partitura tenga exactamente 24 compases correctos:
    - Si hay compases rítmicamente incompletos, ajustá su duración desde **Propiedades del compás**.
    - Si falta contenido, insertá compases (`Ins`) y completalos con silencios o con las notas faltantes.
    - Si sobra un compás vacío, eliminalo con `Ctrl + Supr` (no con `Supr`).

3. **Anacrusa y cierre.** Convertí el primer compás en una anacrusa de una corchea (en 4/4). Verificá que el último compás se ajuste automáticamente para compensar la duración restante. La numeración de compases debe comenzar en el primer compás completo (no en la anacrusa).

4. **Inserta una sección nueva.** Entre los compases 12 y 13 (después de corregir la estructura), insertá 4 compases nuevos (`Ctrl + Ins` → 4). En esos 4 compases, componé una melodía breve de 4 compases en el mismo estilo y tonalidad de la partitura.

5. **Cambio de compás.** A partir del compás 17 (considerando los compases que insertaste), cambiá la indicación de compás a 6/8. Completá los compases restantes con un nuevo material rítmico en 6/8 que tenga sentido musical y cuadre perfectamente con la métrica.

6. **Barras divisorias.** Agregá una **doble barra** justo antes del cambio a 6/8 (entre el último compás en 4/4 y el primero en 6/8). Colocá una **barra final** al terminar la partitura.

7. **Numeración.** Configurá la numeración de compases para que:
    - La anacrusa quede excluida del conteo.
    - Los números sean visibles al inicio de cada sistema.
    - La numeración sea continua (no se reinicie en el cambio de compás).

### Entregables

- [ ] `APELLIDO_Nombre_S06_corregido_v01.mscz` (partitura con estructura corregida)
- [ ] `APELLIDO_Nombre_S06_corregido_v01.pdf`
- [ ] Hoja de auditoría con la lista de problemas detectados (compás y descripción)
- [ ] Captura de pantalla mostrando la doble barra y el cambio a 6/8 con los números de compás visibles

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Corrección estructural | La partitura tiene 24 compases correctos; no hay compases incompletos ni vacíos no previstos | 1–2 compases aún con problemas | ≥3 compases con errores estructurales |
| Anacrusa y cierre | La anacrusa dura una corchea; el último compás se compensó correctamente; la numeración excluye la anacrusa | La anacrusa se creó pero el cierre no se ajustó | No realizó la anacrusa o la duración no coincide |
| Inserción y nueva sección | Insertó 4 compases en la posición correcta; la melodía nueva tiene sentido musical | Insertó los compases pero la melodía es incoherente | No insertó los compases |
| Cambio a 6/8 | El cambio de compás está en la posición correcta; los compases en 6/8 cuadran rítmicamente con la nueva métrica | El cambio existe pero los compases no cuadran con 6/8 | No realizó el cambio de compás |
| Barras divisorias | Doble barra antes del cambio métrico; barra final al terminar; ambas visibles en el PDF | Solo una de las dos barras está presente | No agregó barras divisorias |
| Numeración | Anacrusa excluida; números en cada sistema; numeración continua | Falta uno de los tres criterios | No configuró la numeración |

---

*Basado en: MuseScore Studio 4 Handbook — Time signatures, Barlines, Measure properties, Measure numbering, Pickup and non-metered measures; MuseScore 3 Handbook — Notation: Time signatures, Measure operations, Barlines, Measure rests, Measure numbering | https://handbook.musescore.org*
