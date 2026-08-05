# Sesión 5: Edición y selección

📚 Handbook → Basics: Selecting elements, Copy and paste, Editing notes and rests; Notation → Transposition; Basics → Adding and removing measures | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

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

    En MuseScore, casi todo lo que querés modificar —cambiar altura, transponer, copiar, eliminar— empieza por una **selección precisa**. Una selección incorrecta produce resultados inesperados. Por eso, antes de editar, preguntate: *¿estoy seleccionando exactamente lo que quiero modificar?*

    ### Tipos de selección

    | Tipo | Cómo se hace | Cuándo usarlo |
    |---|---|---|
    | **Un elemento** | Clic sobre la cabeza de la nota, el silencio o el símbolo | Corregir una nota individual, cambiar una dinámica suelta |
    | **Lista de elementos** | `Ctrl + clic` sobre cada elemento (Windows/Linux) o `Cmd + clic` (macOS) | Seleccionar notas o símbolos que NO son contiguos |
    | **Rango continuo** | Clic en la primera nota → `Shift + clic` en la última | Copiar una frase, transponer una sección, eliminar varios compases |
    | **Compás completo** | Clic en un espacio vacío del compás (no sobre una nota) | Insertar, eliminar o duplicar compases enteros |
    | **Seleccionar todo** | `Ctrl + A` (`Cmd + A` en macOS) | Transponer la partitura completa, cambiar el tempo de toda la obra |
    | **Extender con teclado** | `Shift + ←`/`Shift + →` para extender nota por nota; `Shift + Ctrl + ←`/`→` para compás por compás | Extender la selección sin usar el ratón |

    > Insertar captura de una selección de rango: varios compases resaltados con el rectángulo azul característico, mostrando que abarca múltiples pentagramas.

    ### Diferencia visual: nota seleccionada vs. compás seleccionado

    - **Nota seleccionada**: la cabeza de la nota se vuelve azul. Solo esa nota está seleccionada.
    - **Compás seleccionado**: aparece un **rectángulo azul** alrededor de todo el compás. Todas las notas, silencios, articulaciones y símbolos dentro de ese compás están seleccionados.
    - **Rango seleccionado**: el rectángulo azul abarca varios compases y posiblemente varios pentagramas.

    !!! warning "Clic en el lugar correcto"
        Hacer clic sobre una nota selecciona ESA nota. Hacer clic en el espacio vacío del compás selecciona TODO el compás. Si hacés clic en el borde entre dos pentagramas, podrías seleccionar el pentagrama equivocado. La diferencia es sutil pero determina el resultado de la operación que hagas a continuación.

    ### Filtro de selección

    El panel **Ver → Filtro de selección** permite excluir tipos de elementos al copiar o eliminar. Por ejemplo, podés copiar SOLO las notas de un pasaje sin arrastrar las dinámicas ni el texto. O eliminar todo lo que esté en voz 2 sin tocar la voz 1.

    Para usarlo:
    1. Hacé la selección de rango normalmente.
    2. Abrí el filtro de selección (`Ver → Filtro de selección`).
    3. Desmarcá los tipos de elementos que NO querés incluir.
    4. Ejecutá la operación (copiar, cortar, eliminar).

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

    1. Seleccioná el rango que querés copiar (clic en primera nota → `Shift + clic` en última).
    2. Presioná `Ctrl + C` para copiar.
    3. Seleccioná la primera nota o silencio del **destino** (donde querés que se pegue).
    4. Presioná `Ctrl + V` para pegar.

    El contenido pegado **reemplaza** lo que hubiera en el destino. Si pegás 4 compases sobre 2 compases existentes, los últimos 2 se sobrescriben y los primeros 2 se insertan desplazando el resto.

    > Insertar captura del proceso de copiar y pegar: selección de 4 compases (rectángulo azul) en el pentagrama superior, y resultado pegado en el pentagrama inferior.

    ### Repetir con `R`

    La tecla `R` es un atajo específico de MuseScore: **repite la selección inmediatamente después de sí misma**. Es ideal para duplicar patrones rítmicos, ostinatos o frases que se repiten.

    1. Seleccioná el elemento o rango que querés repetir.
    2. Presioná `R`.
    3. El contenido se duplica justo a continuación.

    ### Cortar para mover

    Para mover un pasaje de un lugar a otro:

    1. Seleccioná el rango que querés mover.
    2. Presioná `Ctrl + X` (cortar). El contenido desaparece.
    3. Seleccioná la primera nota del destino.
    4. Presioná `Ctrl + V` (pegar). El contenido aparece en la nueva ubicación.

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
    | 1 | Seleccioná el pasaje cuyas alturas querés cambiar |
    | 2 | Activá el modo Re-pitch: `Ctrl + Shift + I` (`Cmd + Shift + I` en macOS) |
    | 3 | Ingresá las nuevas alturas con el teclado (`A`–`G`). Las duraciones permanecen intactas. |
    | 4 | Salí del modo Re-pitch volviendo al modo Step time |

    ### Escritura enarmónica

    Dos notas que suenan igual pero se escriben diferente (Fa♯ y Sol♭) son **enarmónicas**. MuseScore a veces elige una escritura que no es la más adecuada para el contexto musical (por ejemplo, escribe Mi♯ cuando musicalmente corresponde Fa).

    Para cambiar la escritura enarmónica de una nota:
    1. Seleccioná la nota.
    2. Presioná `J`.

    MuseScore alternará entre las escrituras enarmónicas posibles. Si necesitás más control, usá **Herramientas → Reescribir alturas** o el panel de propiedades.

    > Insertar captura del cambio enarmónico: una nota de Fa♯ seleccionada, y al presionar `J` se convierte en Sol♭, mostrando el cambio visual en el pentagrama.

???+ note "Transposición e inserción/eliminación de compases"

    ### Transponer una selección

    La transposición cambia la altura de todas las notas seleccionadas por un mismo intervalo.

    **Con teclado** (método rápido):
    - Seleccioná el rango → `↑` / `↓` para subir/bajar por semitonos.
    - Seleccioná el rango → `Ctrl + ↑` / `Ctrl + ↓` para subir/bajar por octavas.

    **Con el diálogo de transposición** (método preciso):
    1. Seleccioná el rango que querés transponer (o nada para transponer toda la partitura).
    2. Andá a **Herramientas → Transponer...**.
    3. Elegí entre:
       - **Cromáticamente**: por semitonos. Podés indicar "a tonalidad" (ej. de Do mayor a Re mayor) o "por intervalo" (ej. segunda mayor ascendente).
       - **Diatónicamente**: por grados dentro de la escala. Las relaciones interválicas pueden cambiar.
    4. Marcá "Transponer armaduras" si querés que la armadura también cambie.
    5. Clic en **OK**.

    > Insertar captura del diálogo de transposición: ventana de Herramientas → Transponer con las opciones "Cromáticamente" / "Diatónicamente", el selector de intervalo y los checkboxes de "Transponer armaduras" y "Transponer símbolos de acordes".

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
        Si querés quitar un compás que sobra, usá `Ctrl + Supr`. Si solo querés vaciarlo, usá `Supr`.

---

## Actividad en Classroom

### Tarea: S05 — Edición, corrección y transposición

> **Material necesario**: el docente proporcionará un archivo `ejercicio_S05_correccion.mscz` con una partitura de aproximadamente 24 compases para flauta que contiene al menos **diez errores** intencionales de distinto tipo.

1. **Detección de errores.** Abrí el archivo `ejercicio_S05_correccion.mscz` y reproducilo completo. Identificá todos los errores que encuentres. Los tipos de errores incluyen:
    - Notas con altura incorrecta (desplazadas un grado o un semitono).
    - Duración incorrecta (negra donde debería ser corchea, blanca donde debería ser negra, etc.).
    - Alteraciones faltantes o sobrantes.
    - Compases rítmicamente incompletos o con más tiempos de los que indica la métrica.
    - Silencios mal ubicados o faltantes.

2. **Corrección de errores.** Corregí cada error usando el método más adecuado:
    - Para errores de altura: seleccioná la nota y usá `↑`/`↓` o ingresá la altura correcta.
    - Para errores de duración: seleccioná la nota y usá `Shift + W`/`Shift + Q`.
    - Para errores de compás: insertá o eliminá compases según corresponda (`Ins`, `Ctrl + Ins`, `Ctrl + Supr`).

3. **Reescritura enarmónica.** Localizá dos notas en la partitura donde la escritura enarmónica actual sea incómoda o inusual (ej. Mi♯ en lugar de Fa, o Do♭ en lugar de Si). Seleccionalas y presioná `J` para cambiarlas a su equivalente enarmónico más natural. Documentá el cambio: anotá qué nota era y en qué se convirtió.

4. **Cambio de melodía conservando el ritmo.** Seleccioná los compases 9 a 16. Activá el modo Re-pitch (`Ctrl + Shift + I`) y cambiá todas las alturas de esa sección por una nueva melodía inventada por vos, **sin modificar ninguna duración ni ningún ritmo**. La nueva melodía debe tener sentido musical (no es necesario que sea aleatoria).

5. **Copia entre instrumentos.** Copiá los compases 1 a 8 de la flauta y pegalos en los compases 17 a 24. Luego, con el filtro de selección activado, seleccioná los compases 17 a 24 pero excluí las dinámicas y articulaciones para que solo se copien las notas. Pegá el resultado en una nueva partitura para clarinete en Si♭.

6. **Transposición.** Seleccioná toda la partitura corregida (`Ctrl + A`). Usá **Herramientas → Transponer** para subirla una segunda mayor (2 semitonos). Guardá esta versión como un nuevo archivo.

7. **Registro de modificaciones.** Elaborá una tabla con todas las modificaciones que realizaste sobre el archivo original, indicando para cada una: número de compás, tipo de error encontrado, y la corrección aplicada.

### Entregables

- [ ] `APELLIDO_Nombre_S05_corregido_v01.mscz` (archivo con los 10 errores corregidos)
- [ ] `APELLIDO_Nombre_S05_transpuesto_v01.mscz` (archivo transpuesto una segunda mayor arriba)
- [ ] `APELLIDO_Nombre_S05_corregido_v01.pdf`
- [ ] `APELLIDO_Nombre_S05_transpuesto_v01.pdf`
- [ ] Tabla de modificaciones (PDF o Google Docs) con las correcciones documentadas
- [ ] Nota sobre los cambios enarmónicos realizados (qué nota era, en qué se convirtió)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Detección de errores | Detectó y corrigió ≥8 de los 10 errores; las correcciones son precisas | Detectó 5–7 errores | ≤4 errores detectados |
| Reescritura enarmónica | Cambió correctamente 2 notas con `J` y documentó el cambio | Cambió 1 nota o no documentó | No realizó cambios enarmónicos |
| Re-pitch | La nueva melodía (c. 9–16) tiene alturas diferentes pero las duraciones son exactamente las originales | Alguna duración se modificó accidentalmente | No usó el modo Re-pitch o las duraciones cambiaron |
| Copia entre instrumentos | La copia se realizó correctamente; usó el filtro de selección adecuadamente | La copia se hizo pero sin usar el filtro de selección | No realizó la copia |
| Transposición | La partitura transpuesta está una segunda mayor arriba; las armaduras y alteraciones se ajustaron correctamente | Transposición aplicada pero con errores en las alteraciones resultantes | No realizó la transposición |
| Tabla de modificaciones | Tabla completa con compás, tipo de error y corrección para cada modificación | Tabla incompleta o sin detalle | No entregó la tabla |

---

*Basado en: MuseScore 3 Handbook — Basics: Selecting elements, Copy and paste, Undo and redo; MuseScore Studio Handbook — Selecting elements, Copy and paste, Editing notes and rests, Adding and removing measures | https://musescore.org/en/handbook/3*
