# Sesión 7: Claves, armaduras y alteraciones

📚 Handbook → Notation: Pitch — Clefs, Key signatures, Transposition, Respell pitches; Notation: Instruments, staves & systems — Staff/Part properties | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="clave"></a> **Clave (clef)** | Símbolo colocado al inicio del pentagrama que asigna un nombre de nota a cada línea y espacio. Las más comunes: clave de sol (Sol en segunda línea), clave de fa (Fa en cuarta línea), clave de do en tercera (alto) y clave de do en cuarta (tenor). |
    | <a id="cambio-clave"></a> **Cambio de clave** | Sustitución de una clave por otra en el transcurso de la partitura. MuseScore reposiciona automáticamente las notas siguientes para que mantengan su altura real; la clave nueva solo cambia cómo se visualizan. |
    | <a id="armadura"></a> **Armadura de clave (key signature)** | Conjunto de sostenidos o bemoles escritos al inicio del pentagrama (y después de cada cambio de tonalidad) que indican las alteraciones propias de una tonalidad. Afecta a todas las notas de ese nombre en cualquier octava. |
    | <a id="tonalidad"></a> **Tonalidad (key)** | Sistema de organización musical definido por una tónica y un modo (mayor o menor). La armadura es su representación gráfica en la partitura. |
    | <a id="alteracion-propia"></a> **Alteración propia** | Sostenido o bemol que pertenece a la armadura de la tonalidad y se aplica automáticamente a todas las notas de ese nombre. No se escribe delante de cada nota; está implícito en la armadura. |
    | <a id="alteracion-accidental"></a> **Alteración accidental** | Alteración que no pertenece a la armadura y se escribe explícitamente delante de una nota. Afecta a todas las notas del mismo nombre y altura dentro del mismo compás. |
    | <a id="alteracion-precaucion"></a> **Alteración de precaución / cortesía** | Alteración entre paréntesis que se escribe para recordar al intérprete que una alteración previa ya no tiene efecto. MuseScore las añade automáticamente, por ejemplo, en el primer compás de un nuevo sistema si una nota fue alterada en el compás anterior. |
    | <a id="becuadro"></a> **Becuadro (natural)** | Signo (♮) que cancela cualquier alteración previa (propia o accidental). Devuelve la nota a su altura natural. Se ingresa con la tecla `=` en el modo de ingreso. |
    | <a id="transposicion-escrita"></a> **Afinación escrita vs. afinación de concierto** | En los instrumentos transpositores, la partitura se escribe en una tonalidad distinta a la que realmente suena. La **afinación de concierto** muestra las alturas reales; la **afinación escrita** muestra lo que lee el instrumentista. El botón "Concert pitch" en la barra de estado alterna entre ambas vistas. |

???+ note "Claves: tipos, cambios y usos instrumentales"

    ### Las claves principales y sus instrumentos

    | Clave | Línea de referencia | Instrumentos típicos |
    |---|---|---|
    | Sol (𝄞) | Segunda línea (Sol₄) | Violín, flauta, oboe, clarinete, trompeta, piano (mano derecha), guitarra, voz soprano |
    | Fa (𝄢) | Cuarta línea (Fa₃) | Contrabajo, violonchelo, fagot, trombón, tuba, piano (mano izquierda), voz bajo |
    | Do en tercera (alto) | Tercera línea (Do₄) | Viola, trombón alto |
    | Do en cuarta (tenor) | Cuarta línea (Do₄) | Violonchelo (registro agudo), fagot (registro agudo), trombón tenor |

    ### Agregar o cambiar la clave inicial

    Para cambiar la clave del primer compás de un pentagrama:
    1. Seleccionar la clave inicial o el primer compás.
    2. Elegir la clave deseada en la paleta **Claves**.

    También podés arrastrar la clave desde la paleta hasta el primer compás.

    ### Insertar un cambio de clave a mitad de la partitura

    1. Seleccionar una nota, silencio o compás (excepto el primero).
    2. Hacer clic en la clave deseada en la paleta **Claves**.


    !!! tip "Un cambio de clave no transpone: reposiciona"
        Al insertar un cambio de clave, MuseScore **no cambia la altura de las notas**. Simplemente las reubica visualmente para que sigan sonando igual. Si un Do₄ estaba en la primera línea adicional inferior en clave de sol, al cambiar a clave de fa aparecerá en el segundo espacio (pero seguirá siendo Do₄).

    ### Eliminar un cambio de clave

    Seleccionar la clave insertada y presionar `Supr`. Las claves iniciales de cada sistema no se pueden eliminar.

    ### Claves de cortesía

    Cuando un cambio de clave coincide con el inicio de un sistema nuevo, MuseScore muestra automáticamente una clave de cortesía (más pequeña) al final del sistema anterior. Esto se configura en **Formato → Estilo → Claves, armaduras e indicaciones de compás**.

???+ note "Armaduras y cambios de tonalidad"

    ### Agregar o cambiar la armadura

    1. Seleccionar un compás, nota, silencio o armadura existente.
    2. Elegir la armadura en la paleta **Armaduras**.

    Los cambios de armadura ocurren al inicio del compás. Sin embargo, también es posible insertarlos a mitad de un compás sobre una nota específica.

    ### El círculo de quintas en la paleta

    La paleta de armaduras organiza las tonalidades en orden creciente de alteraciones:

    | Sostenidos | Tonalidad mayor | Tonalidad menor relativa |
    |---|---|---|
    | 0 | Do mayor | La menor |
    | 1 ♯ | Sol mayor | Mi menor |
    | 2 ♯ | Re mayor | Si menor |
    | 3 ♯ | La mayor | Fa♯ menor |
    | 4 ♯ | Mi mayor | Do♯ menor |
    | 5 ♯ | Si mayor | Sol♯ menor |
    | 6 ♯ | Fa♯ mayor | Re♯ menor |

    | Bemoles | Tonalidad mayor | Tonalidad menor relativa |
    |---|---|---|
    | 1 ♭ | Fa mayor | Re menor |
    | 2 ♭ | Si♭ mayor | Sol menor |
    | 3 ♭ | Mi♭ mayor | Do menor |
    | 4 ♭ | La♭ mayor | Fa menor |
    | 5 ♭ | Re♭ mayor | Si♭ menor |
    | 6 ♭ | Sol♭ mayor | Mi♭ menor |


    ### Eliminar una armadura

    Seleccionar la armadura y presionar `Supr`. No se puede eliminar la armadura del primer compás del score: MuseScore interpreta eso como "no sé si querés Do mayor o atonal". Si querés Do mayor, simplemente seleccioná la armadura de Do mayor desde la paleta.

    ### Armaduras de cortesía

    Al igual que con los cambios de compás, MuseScore muestra armaduras de cortesía al final del sistema anterior cuando un cambio de tonalidad coincide con el inicio de un sistema. Se configuran en **Formato → Estilo → Claves, armaduras e indicaciones de compás**.

    ### Armadura local (por pentagrama)

    En algunos scores puede necesitarse una armadura diferente para un pentagrama específico. Para añadir una armadura local:
    1. Mantener `Ctrl` (`Cmd` en macOS).
    2. Arrastrar la armadura desde la paleta al pentagrama correspondiente.

    ### Armadura abierta / atonal

    Algunos instrumentos (trompa, timbales) se escriben convencionalmente sin armadura aunque la obra esté en una tonalidad definida. La armadura "abierta/atonal" se ve igual que Do mayor pero no se ve afectada por la transposición. Se aplica como armadura local.

???+ note "Alteraciones: propias, accidentales y de precaución"

    ### Tipos de alteración

    | Alteración | Tecla | Símbolo | Efecto |
    |---|---|---|---|
    | Sostenido | `+` | ♯ | Sube un semitono |
    | Bemol | `-` | ♭ | Baja un semitono |
    | Becuadro | `=` | ♮ | Cancela alteraciones previas |
    | Doble sostenido | (paleta) | 𝄪 | Sube dos semitonos |
    | Doble bemol | (paleta) | 𝄫 | Baja dos semitonos |

    Las alteraciones se ingresan en modo de ingreso de notas **antes** de la nota. La secuencia es: duración → alteración → altura (`5` → `+` → `F` produce un Fa♯ negra).

    ### Reglas de comportamiento de las alteraciones

    1. **Alteración propia**: la armadura define qué notas son alteradas por defecto en toda la partitura. Si la armadura tiene Fa♯, todos los Fa (en cualquier octava) son Fa♯ sin necesidad de escribirlo.

    2. **Alteración accidental**: una alteración escrita delante de una nota **anula** la alteración propia para esa nota y todas las del mismo nombre y altura dentro del mismo compás. Ejemplo: en Sol mayor (Fa♯ en la armadura), si escribís un Fa♮, todos los Fa siguientes en ese compás también serán Fa♮.

    3. **Cambio de compás**: al cruzar la barra divisoria, TODAS las alteraciones accidentales se cancelan automáticamente. En el compás siguiente, la armadura vuelve a regir.

    4. **Alteración de precaución**: MuseScore añade automáticamente alteraciones entre paréntesis cuando una nota alterada en un compás aparece sin alteración en el compás siguiente, para evitar confusiones.

    !!! tip "Las alteraciones de precaución son automáticas"
        No necesitás ingresarlas manualmente. MuseScore las coloca automáticamente según las reglas de cortesía. Si querés ocultar una alteración de precaución específica, seleccionala y en el panel **Propiedades** desmarcá su visibilidad o presioná `V`.

    ### Cambiar la altura de una nota ya escrita

    | Operación | Atajo |
    |---|---|
    | Subir un semitono | `↑` |
    | Bajar un semitono | `↓` |
    | Subir diatónicamente | `Alt + Shift + ↑` |
    | Bajar diatónicamente | `Alt + Shift + ↓` |
    | Subir una octava | `Ctrl + ↑` |
    | Bajar una octava | `Ctrl + ↓` |

    ### Escritura enarmónica

    Dos notas que suenan igual pero se escriben diferente (ej. Fa♯ y Sol♭) son **enarmónicas**. Para cambiar la escritura enarmónica de una nota: seleccionala y presioná `J`. MuseScore alternará entre las representaciones disponibles.

???+ note "Transposición e instrumentos transpositores"

    ### Transponer una selección

    **Método rápido con teclado:**
    - `↑` / `↓`: subir/bajar por semitonos.
    - `Ctrl + ↑` / `Ctrl + ↓`: subir/bajar por octavas.

    **Método preciso con diálogo:**
    1. Seleccionar el rango (o nada para transponer todo).
    2. **Herramientas → Transponer...**
    3. Elegir entre:
       - **Cromáticamente**: por semitonos. Opciones: "A tonalidad" o "Por intervalo".
       - **Diatónicamente**: por grados de la escala.
    4. Marcar **Transponer armaduras** si la tonalidad también debe cambiar.
    5. Clic en **OK**.


    ### Instrumentos transpositores

    Algunos instrumentos se escriben en una tonalidad diferente a la que realmente suenan. Esto permite que el instrumentista use siempre la misma digitación.

    | Instrumento | Afinación | Si la obra está en Do mayor, la parte se escribe en... |
    |---|---|---|
    | Clarinete en Si♭ | Un tono abajo | Re mayor (un tono arriba) |
    | Saxofón alto en Mi♭ | Una sexta mayor abajo | La mayor (una sexta mayor arriba) |
    | Trompeta en Si♭ | Un tono abajo | Re mayor (un tono arriba) |
    | Corno en Fa | Una quinta justa abajo | Sol mayor (una quinta justa arriba) |

    ### Afinación de concierto vs. afinación escrita

    El botón **Concert pitch** (a la izquierda del icono del diapasón en la barra de estado) alterna entre:
    - **Activado**: muestra todas las partes en altura real (Do mayor se ve Do mayor en todos los pentagramas).
    - **Desactivado**: muestra las partes en altura escrita (el clarinete en Si♭ se ve en Re mayor cuando la obra está en Do mayor).

    !!! important "Verificá siempre la vista correcta"
        Al crear un score con instrumentos transpositores, MuseScore configura automáticamente la transposición de cada pentagrama. Pero al exportar partes individuales, asegurate de que **Concert pitch esté desactivado** para que cada instrumentista reciba su parte en la tonalidad escrita correcta.

    ### Configurar la transposición de un pentagrama manualmente

    Si por algún motivo necesitás ajustar la transposición de un instrumento:
    1. Clic derecho en el pentagrama → **Propiedades de pentagrama/parte**.
    2. En **Transposición**, seleccionar el intervalo que el instrumento transpone **hacia abajo** desde la afinación de concierto.
    3. Para clarinete en Si♭: "Seconda mayor descendente" (suena un tono abajo de lo escrito).

---

## Actividad en Classroom

### Tarea: S07 — Claves, armaduras y transposición

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S07_claves.mscz`, una partitura para violín en Do mayor, 4/4, 16 compases con una melodía diatónica; (b) `ejercicio_S07_transposicion.mscz`, una partitura para flauta en Do mayor con pasajes que requieren transposición.

1. **Cambios de clave en un mismo pentagrama.** Abrí `ejercicio_S07_claves.mscz`. Insertá los siguientes cambios de clave en el pentagrama del violín:
    - Compás 5: cambiá a clave de Do en tercera (alto).
    - Compás 9: cambiá a clave de Fa en cuarta.
    - Compás 13: regresá a clave de Sol.
    - Verificá que las alturas sigan siendo las mismas (las notas se reposicionaron pero suenan igual).

2. **Armaduras y cambios de tonalidad.** Sobre la misma partitura:
    - En el compás 1, cambiá la armadura de Do mayor a Sol mayor (1 sostenido). Observá cómo los Fa existentes se convierten en Fa♯ automáticamente.
    - En el compás 9, insertá un cambio de armadura a Fa mayor (1 bemol). El Si pasa a ser Si♭.
    - En el compás 13, regresá a Do mayor.
    - Insertá dobles barras antes de cada cambio de armadura para señalar las secciones.

3. **Alteraciones accidentales.** En los compases 2 y 6 de la partitura en Sol mayor, escribí al menos:
    - Un Fa♮ (becuadro que cancela el Fa♯ de la armadura).
    - Un Do♯ (sostenido accidental).
    - Verificá que al cruzar la barra del compás, las alteraciones accidentales desaparezcan. En el compás siguiente, ¿el Fa volvió a ser Fa♯?

4. **Transposición de melodía.** Abrí `ejercicio_S07_transposicion.mscz`. Seleccioná toda la partitura (`Ctrl + A`). Usá **Herramientas → Transponer** para:
    - Subirla una **segunda mayor ascendente** (2 semitonos). Marcá "Transponer armaduras".
    - Guardar como archivo nuevo.
    - Deshacer (`Ctrl + Z`) y luego transponer **diatónicamente** una tercera arriba. Comparar el resultado con la transposición cromática: ¿en qué se diferencian?

5. **Instrumento transpositor.** Creá una partitura nueva para **clarinete en Si♭**. Copiá los compases 1 a 8 de la flauta del ejercicio `S07_transposicion` original (el de Do mayor) y pegalos en el clarinete:
    - ¿En qué tonalidad se escribe el clarinete? ¿Por qué?
    - Activá el botón **Concert pitch** y observá qué cambia visualmente. Desactivalo de nuevo.
    - Verificá que la armadura del clarinete sea la correcta para que suene en Do mayor.

6. **Informe de observaciones.** Elaborá un breve documento (media página) donde expliques con tus palabras:
    - ¿Qué diferencia hay entre una alteración propia y una accidental?
    - ¿Para qué sirve una alteración de precaución?
    - ¿Por qué el clarinete en Si♭ necesita una armadura distinta a la flauta para sonar en la misma tonalidad?

### Entregables

- [ ] `APELLIDO_Nombre_S07_claves_v01.mscz` (partitura con cambios de clave, armadura y alteraciones)
- [ ] `APELLIDO_Nombre_S07_claves_v01.pdf`
- [ ] `APELLIDO_Nombre_S07_transpuesto_v01.mscz` (transposición segunda mayor arriba)
- [ ] `APELLIDO_Nombre_S07_transpuesto_v01.pdf`
- [ ] `APELLIDO_Nombre_S07_clarinete_v01.mscz` (partitura con parte de clarinete en Si♭)
- [ ] `APELLIDO_Nombre_S07_clarinete_v01.pdf`
- [ ] Informe de observaciones (media página, PDF o Google Docs)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Cambios de clave | Los tres cambios de clave están insertados en los compases correctos; las alturas suenan igual que el original | 1–2 cambios correctos; alguna altura se alteró | No realizó los cambios de clave o las alturas no coinciden |
| Armaduras | Los tres cambios de armadura son correctos (Sol M, Fa M, Do M); dobles barras presentes | 1–2 cambios correctos; faltan barras divisorias | Cambios incorrectos o no realizados |
| Alteraciones accidentales | Fa♮ y Do♯ correctamente ingresados; las alteraciones se cancelan al cruzar el compás | Una alteración ausente o no se verificó el comportamiento | No ingresó alteraciones |
| Transposición | La partitura está transpuesta correctamente (segunda mayor); la armadura cambió junto con las notas | Transposición aplicada pero con errores en la armadura resultante | Transposición no realizada |
| Clarinete en Si♭ | La parte de clarinete está en Re mayor (un tono arriba); las alturas suenan igual que la flauta | El clarinete tiene la armadura correcta pero hay discrepancias de altura | No creó la parte de clarinete o la armadura es incorrecta |
| Informe | Explica con claridad los tres conceptos; usa ejemplos del ejercicio | Explica 2 de 3 conceptos | No entregó el informe |

---

*Basado en: MuseScore Studio 4 Handbook — Clefs, Key signatures, Transposition, Respell pitches; MuseScore 3 Handbook — Notation: Clefs, Key signatures, Accidentals, Transposition | https://handbook.musescore.org*
