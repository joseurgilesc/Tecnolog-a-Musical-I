# Sesión 5: Edición y selección

📚 Handbook → Basics: Selecting elements, Copy and paste, Editing notes and rests; Notation → Transposition; Basics → Adding and removing measures | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consulta esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="seleccion"></a> **Selección** | Acción de marcar uno o más elementos de la partitura para editarlos, copiarlos o eliminarlos. Puede ser de un solo elemento, una lista de elementos sueltos o un rango continuo de compases. |
    | <a id="rango"></a> **Rango de selección** | Selección que abarca todos los elementos entre un punto de inicio y un punto final, incluyendo notas, silencios, articulaciones y texto. Se representa como un rectángulo azul sobre la región seleccionada. |
    | <a id="enharmonia"></a> **Enarmonía** | Relación entre dos notas que suenan igual pero se escriben diferente (ej. Fa♯ y Sol♭). MuseScore permite cambiar la escritura enarmónica de una nota con la tecla `J`. |
    | <a id="transposicion"></a> **Transposición** | Operación que cambia la altura de una selección de notas por un intervalo fijo, manteniendo las relaciones entre ellas. Puede ser cromática (por semitonos) o diatónica (por grados de la escala). |
    | <a id="filtro-seleccion"></a> **Filtro de selección** | Panel que permite incluir o excluir tipos específicos de elementos (voz 1, voz 2, dinámicas, texto, etc.) en una selección de rango. Se activa desde **Ver → Filtro de selección**. |
    | <a id="portapapeles"></a> **Portapapeles** | Espacio de memoria temporal donde se almacenan los elementos copiados o cortados. Se accede con `Ctrl + C` (copiar), `Ctrl + X` (cortar) y `Ctrl + V` (pegar). |
    | <a id="insertar-compas"></a> **Insertar compás** | Agregar uno o más compases vacíos en una posición específica de la partitura, desplazando el contenido existente hacia adelante. Atajo: `Ins` para un compás, `Ctrl + Ins` para varios. |
    | <a id="eliminar-compas"></a> **Eliminar compás** | Suprimir uno o más compases completos junto con todo su contenido. Atajo: `Ctrl + Supr` (`Cmd + Supr` en macOS). No debe confundirse con borrar las notas dentro del compás (`Supr`). |
    | <a id="modo-normal"></a> **Modo normal** | Estado por defecto de MuseScore fuera del modo de ingreso de notas. En este modo se realizan la mayoría de las operaciones de edición: seleccionar, copiar, pegar, transponer, eliminar compases. |
    | <a id="re-pitch"></a> **Modo Re-pitch** | Modo de ingreso alternativo que permite cambiar las alturas de una secuencia de notas manteniendo intactas sus duraciones y ritmo. Se activa con `Ctrl + Shift + I` (`Cmd + Shift + I` en macOS). |

???+ note "Selección: la base de toda edición"

    En MuseScore, casi todo lo que quieres modificar —cambiar altura, transponer, copiar, eliminar— empieza por una **selección precisa**. Una selección incorrecta produce resultados inesperados. Por eso, antes de editar, pregúntate: *¿estoy seleccionando exactamente lo que quiero modificar?*

    ### Tipos de selección

    | Tipo | Cómo se hace | Cuándo usarlo |
    |---|---|---|
    | **Un elemento** | Clic sobre la cabeza de la nota, el silencio o el símbolo | Corregir una nota individual, cambiar una dinámica suelta |
    | **Lista de elementos** | `Ctrl + clic` sobre cada elemento (Windows/Linux) o `Cmd + clic` (macOS) | Seleccionar notas o símbolos que NO son contiguos |
    | **Rango continuo** | Clic en la primera nota → `Shift + clic` en la última | Copiar una frase, transponer una sección, eliminar varios compases |
    | **Compás completo** | Clic en un espacio vacío del compás (no sobre una nota) | Insertar, eliminar o duplicar compases enteros |
    | **Seleccionar todo** | `Ctrl + A` (`Cmd + A` en macOS) | Transponer la partitura completa, cambiar el tempo de toda la obra |
    | **Extender con teclado** | `Shift + ←`/`Shift + →` para extender nota por nota; `Shift + Ctrl + ←`/`→` para compás por compás | Extender la selección sin usar el ratón |


    ### Diferencia visual: nota seleccionada vs. compás seleccionado

    - **Nota seleccionada**: la cabeza de la nota se vuelve azul. Solo esa nota está seleccionada.
    - **Compás seleccionado**: aparece un **rectángulo azul** alrededor de todo el compás. Todas las notas, silencios, articulaciones y símbolos dentro de ese compás están seleccionados.
    - **Rango seleccionado**: el rectángulo azul abarca varios compases y posiblemente varios pentagramas.

    !!! warning "Clic en el lugar correcto"
        Hacer clic sobre una nota selecciona ESA nota. Hacer clic en el espacio vacío del compás selecciona TODO el compás. Si haces clic en el borde entre dos pentagramas, podrías seleccionar el pentagrama equivocado. La diferencia es sutil pero determina el resultado de la operación que hagas a continuación.

    ### Filtro de selección

    El panel **Ver → Filtro de selección** permite excluir tipos de elementos al copiar o eliminar. Por ejemplo, puedes copiar SOLO las notas de un pasaje sin arrastrar las dinámicas ni el texto. O eliminar todo lo que esté en voz 2 sin tocar la voz 1.

    Para usarlo:
    1. Haz la selección de rango normalmente.
    2. Abre el filtro de selección (`Ver → Filtro de selección`).
    3. Desmarca los tipos de elementos que NO quieres incluir.
    4. Ejecuta la operación (copiar, cortar, eliminar).

???+ note "Copiar, cortar y pegar: el poder de la repetición"

    Copiar y pegar en MuseScore funciona como en cualquier programa, pero con particularidades importantes.

    ### Operaciones básicas

    | Operación | Atajo Windows/Linux | Atajo macOS |
    |---|---|---|
    | Copiar | `Ctrl + C` | `Cmd + C` |
    | Cortar | `Ctrl + X` | `Cmd + X` |
    | Pegar | `Ctrl + V` | `Cmd + V` |
    | Repetir selección | `R` | `R` |
    | Intercambiar con portapapeles | `Ctrl + Shift + X` | `Cmd + Shift + X` |

    ### Procedimiento para copiar un pasaje

    1. Selecciona el rango que quieres copiar (clic en primera nota → `Shift + clic` en última).
    2. Presiona `Ctrl + C` para copiar.
    3. Selecciona la primera nota o silencio del **destino** (donde quieres que se pegue).
    4. Presiona `Ctrl + V` para pegar.

    El contenido pegado **reemplaza** lo que hubiera en el destino. Si pegas 4 compases sobre 2 compases existentes, los últimos 2 se sobrescriben y los primeros 2 se insertan desplazando el resto.


    ### Repetir con `R`

    La tecla `R` es un atajo específico de MuseScore: **repite la selección inmediatamente después de sí misma**. Es ideal para duplicar patrones rítmicos, ostinatos o frases que se repiten.

    1. Selecciona el elemento o rango que quieres repetir.
    2. Presiona `R`.
    3. El contenido se duplica justo a continuación.

    ### Cortar para mover

    Para mover un pasaje de un lugar a otro:

    1. Selecciona el rango que quieres mover.
    2. Presiona `Ctrl + X` (cortar). El contenido desaparece.
    3. Selecciona la primera nota del destino.
    4. Presiona `Ctrl + V` (pegar). El contenido aparece en la nueva ubicación.

    ### Pegar mitad / doble duración

    MuseScore permite pegar un pasaje con las duraciones modificadas:

    | Comando | Atajo | Efecto |
    |---|---|---|
    | Pegar mitad duración | `Ctrl + Shift + Q` | Las corcheas se convierten en semicorcheas, las negras en corcheas, etc. |
    | Pegar doble duración | `Ctrl + Shift + W` | Las corcheas se convierten en negras, las negras en blancas, etc. |

???+ note "Edición de alturas, duraciones y escritura enarmónica"

    Una vez ingresadas las notas, MuseScore ofrece múltiples formas de modificarlas sin borrar y reescribir.

    ### Cambiar altura

    | Operación | Atajo | Efecto |
    |---|---|---|
    | Subir un semitono | `↑` | Sube la altura y escribe con sostenidos (Do → Do♯) |
    | Bajar un semitono | `↓` | Baja la altura y escribe con bemoles (Mi → Mi♭) |
    | Subir diatónicamente | `Alt + Shift + ↑` | Sube un grado de la escala (Do → Re) |
    | Bajar diatónicamente | `Alt + Shift + ↓` | Baja un grado de la escala (Mi → Re) |
    | Subir una octava | `Ctrl + ↑` | Sube la nota 8 grados |
    | Bajar una octava | `Ctrl + ↓` | Baja la nota 8 grados |

    Estos atajos funcionan tanto en modo de ingreso como en modo normal, sobre notas individuales o sobre selecciones de rango.

    ### Cambiar duración

    | Operación | Atajo | Efecto |
    |---|---|---|
    | Aumentar duración | `Shift + W` | Negra → Negra con puntillo → Blanca |
    | Reducir duración | `Shift + Q` | Blanca → Blanca con puntillo → Negra |
    | Duplicar duración | `W` | Corchea → Negra; Negra → Blanca |
    | Reducir a la mitad | `Q` | Negra → Corchea; Blanca → Negra |

    ### Modo Re-pitch: cambiar alturas conservando el ritmo

    El modo **Re-pitch** es uno de los más potentes para edición. Permite reescribir las alturas de un pasaje sin modificar ni una sola duración. Ideal cuando tenés un patrón rítmico complejo y necesitás cambiar la melodía.

    | Paso | Acción |
    |---|---|
    | 1 | Selecciona el pasaje cuyas alturas quieres cambiar |
    | 2 | Activa el modo Re-pitch: `Ctrl + Shift + I` (`Cmd + Shift + I` en macOS) |
    | 3 | Ingresa las nuevas alturas con el teclado (`A`–`G`). Las duraciones permanecen intactas. |
    | 4 | Sal del modo Re-pitch volviendo al modo Step time |

    ### Escritura enarmónica

    Dos notas que suenan igual pero se escriben diferente (Fa♯ y Sol♭) son **enarmónicas**. MuseScore a veces elige una escritura que no es la más adecuada para el contexto musical (por ejemplo, escribe Mi♯ cuando musicalmente corresponde Fa).

    Para cambiar la escritura enarmónica de una nota:
    1. Selecciona la nota.
    2. Presiona `J`.

    MuseScore alternará entre las escrituras enarmónicas posibles. Si necesitas más control, usa **Herramientas → Reescribir alturas** o el panel de propiedades.


???+ note "Transposición e inserción/eliminación de compases"

    ### Transponer una selección

    La transposición cambia la altura de todas las notas seleccionadas por un mismo intervalo.

    **Con teclado** (método rápido):
    - Selecciona el rango → `↑` / `↓` para subir/bajar por semitonos.
    - Selecciona el rango → `Ctrl + ↑` / `Ctrl + ↓` para subir/bajar por octavas.

    **Con el diálogo de transposición** (método preciso):
    1. Selecciona el rango que quieres transponer (o nada para transponer toda la partitura).
    2. Ve a **Herramientas → Transponer...**.
    3. Elige entre:
       - **Cromáticamente**: por semitonos. Puedes indicar "a tonalidad" (ej. de Do mayor a Re mayor) o "por intervalo" (ej. segunda mayor ascendente).
       - **Diatónicamente**: por grados dentro de la escala. Las relaciones interválicas pueden cambiar.
    4. Marca "Transponer armaduras" si quieres que la armadura también cambie.
    5. Clic en **OK**.


    ### Insertar compases

    Insertar un compás agrega espacio vacío y desplaza todo el contenido posterior hacia adelante. Es distinto de **añadir** compases al final.

    | Método | Acción |
    |---|---|
    | **Un compás antes de la selección** | Seleccionar un compás → `Ins` |
    | **Varios compases antes** | `Ctrl + Ins` (`Cmd + Ins`) → ingresar cantidad |
    | **Al final de la partitura** | `Ctrl + B` (`Cmd + B`) para un compás; `Alt + Shift + B` para varios |
    | **Con menú contextual** | Clic derecho en compás → Insertar compases → elegir ubicación y cantidad |

    ### Eliminar compases

    Eliminar un compás suprime el compás completo Y todo su contenido. No es lo mismo que borrar las notas dentro del compás (`Supr`).

    | Método | Acción |
    |---|---|
    | **Con teclado** | Seleccionar compás → `Ctrl + Supr` (`Cmd + Supr` en macOS) |
    | **Con menú contextual** | Clic derecho en compás → Eliminar compases |
    | **Herramientas** | Seleccionar compás → Herramientas → Eliminar rango seleccionado |

    !!! warning "No confundas borrar notas con eliminar compases"
        - `Supr` dentro de un compás: borra las notas y las reemplaza por silencios. El compás sigue existiendo.
        - `Ctrl + Supr` sobre un compás seleccionado: ELIMINA el compás completo. Los compases posteriores se desplazan hacia atrás.
        Si quieres quitar un compás que sobra, usa `Ctrl + Supr`. Si solo quieres vaciarlo, usa `Supr`.

---

## 🎹 Desafío de Shortcuts — Sesión 5

Practica los atajos de edición, selección y compases. Al final verás tus errores para repasarlos en MuseScore.

[🎮 Jugar Desafío S5](../../juegos/shortcuts-game.html?sesion=5){ .md-button .md-button--primary }

---

Ver el ejercicio en Classroom.

---

*Basado en: MuseScore 3 Handbook — Basics: Selecting elements, Copy and paste, Undo and redo; MuseScore Studio Handbook — Selecting elements, Copy and paste, Editing notes and rests, Adding and removing measures | https://musescore.org/en/handbook/3*
