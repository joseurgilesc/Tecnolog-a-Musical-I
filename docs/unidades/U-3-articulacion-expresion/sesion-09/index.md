# Sesión 9: Articulaciones y ornamentos

📚 Handbook → Notation: Expressive markings — Articulations, Ornaments, Slurs and ties | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="articulacion"></a> **Articulación** | Marca que indica cómo debe ser atacada o ejecutada una nota. No cambia la altura ni la duración, sino el carácter del sonido: puede ser corta, acentuada, ligada, pesada, etc. |
    | <a id="staccato"></a> **Staccato** | Punto colocado sobre o bajo la cabeza de la nota. Indica que la nota debe ejecutarse más corta de lo escrito, separándola de la siguiente. Atajo: `Shift + S`. |
    | <a id="tenuto"></a> **Tenuto** | Línea horizontal sobre o bajo la nota. Indica que la nota debe mantenerse durante todo su valor, con un leve énfasis y sin separación. Atajo: `Shift + N`. |
    | <a id="acento"></a> **Acento (accent)** | Signo `>` colocado sobre o bajo la nota. Indica un ataque más fuerte al inicio de la nota, sin acortarla necesariamente. Atajo: `Shift + V`. |
    | <a id="marcato"></a> **Marcato** | Signo `^` (en forma de cuña) sobre o bajo la nota. Indica un ataque aún más marcado y fuerte que el acento. Se ejecuta con más peso y separación. Atajo: `Shift + O`. |
    | <a id="calderon"></a> **Calderón (fermata / pause)** | Semicírculo con un punto debajo (`𝄐`). Indica que la nota o silencio debe sostenerse más tiempo del que indica su figura. La duración exacta queda a criterio del intérprete. |
    | <a id="trino"></a> **Trino (trill)** | Ornamento que consiste en alternar rápidamente entre la nota escrita y la nota superior (generalmente un tono o semitono). Se indica con las letras `tr` seguidas opcionalmente de una línea ondulada. |
    | <a id="mordente"></a> **Mordente** | Ornamento breve que alterna la nota principal con la nota superior (mordente superior) o inferior (mordente inferior, con línea vertical). El mordente superior se escribe como una línea quebrada `M` sin tachar; el inferior tiene una línea vertical que lo cruza. |
    | <a id="grupeto"></a> **Grupeto (turn)** | Ornamento de cuatro notas: nota superior, principal, inferior, principal. Se escribe como una `S` acostada. Puede colocarse directamente sobre una nota (comienza en la superior) o entre dos notas (comienza en la principal). |
    | <a id="ligadura-expresion"></a> **Ligadura de expresión (slur)** | Línea curva que abarca varias notas de diferente altura. Indica que deben ejecutarse de forma ligada (*legato*), sin articulación separada entre ellas. En instrumentos de viento, todas las notas bajo una ligadura se tocan en un solo soplo. |
    | <a id="ligadura-prolongacion"></a> **Ligadura de prolongación (tie)** | Línea curva que conecta dos notas de la misma altura. La segunda nota no se articula; simplemente prolonga la duración de la primera. A diferencia de la ligadura de expresión, une notas del mismo nombre. |

???+ note "Articulaciones: staccato, tenuto, acento, marcato y calderón"

    Las articulaciones son marcas que le dicen al intérprete **cómo atacar cada nota**. No modifican la altura ni la duración escrita, pero sí el carácter y la separación entre sonidos.

    ### Tipos principales de articulación

    | Articulación | Símbolo | Atajo | Efecto en la ejecución |
    |---|---|---|---|
    | Staccato | Punto sobre/bajo la nota | `Shift + S` | Nota más corta, separada |
    | Staccatissimo | Cuña (más aguda que el staccato) | (paleta) | Nota aún más corta y marcada |
    | Tenuto | Línea horizontal | `Shift + N` | Nota sostenida todo su valor, leve énfasis |
    | Acento | `>` | `Shift + V` | Ataque fuerte al inicio |
    | Marcato | `^` | `Shift + O` | Ataque muy fuerte, con peso |

    ### Agregar articulaciones

    Desde la paleta **Articulaciones**:
    1. Seleccionar una o varias notas.
    2. Hacer clic en el símbolo deseado en la paleta.
    3. También se puede arrastrar el símbolo directamente sobre la cabeza de la nota.

    También hay cuatro articulaciones accesibles desde la barra de herramientas de ingreso de notas (acento, marcato, staccato y tenuto).


    ### Reproducción automática

    MuseScore ajusta automáticamente la reproducción según la articulación aplicada:
    - Un **staccato** acorta la nota aproximadamente a la mitad de su duración.
    - Un **acento** aumenta el volumen del ataque inicial.
    - Un **marcato** combina un ataque fuerte con una ligera separación.
    - El **tenuto** asegura que la nota dure su valor completo.

    ### Posición y propiedades

    Seleccionando una articulación podés ajustar en el panel **Propiedades**:
    - **Colocación**: arriba o abajo de la nota. MuseScore elige automáticamente según la dirección de la plica, pero podés forzar la posición manualmente.

    ### Calderón (fermata)

    El calderón indica una pausa o suspensión del pulso sobre una nota, un silencio o una barra de compás. Se encuentra en la paleta **Articulaciones**. En reproducción, MuseScore alarga automáticamente la duración de la nota (por defecto, al doble con un leve *rallentando*), aunque el valor exacto es configurable en el panel **Propiedades**.


    !!! tip "Combinar articulaciones"
        MuseScore permite combinar varias articulaciones sobre una misma nota. Por ejemplo, un tenuto + staccato produce un *portato* (o *louré*): notas separadas pero con peso. Las opciones de alineación (mantener juntas, preferir cercanía a la cabeza) se configuran en **Formato → Estilo → Articulaciones y ornamentos**.

???+ note "Ornamentos: trinos, mordentes y grupetos"

    Los ornamentos son figuras que embellecen una nota principal mediante la adición rápida de notas adyacentes. En MuseScore, se aplican desde la paleta **Ornamentos**.

    ### Trino (trill)

    El trino es una alternancia rápida entre la nota escrita y la nota superior. MuseScore ofrece dos formas:
    - **Trino corto** (de la paleta Ornamentos): el símbolo `tr` sin línea de extensión, adecuado para notas breves.
    - **Línea de trino** (de la paleta Líneas): `tr` seguido de una línea ondulada que se extiende sobre varias notas. Se aplica como cualquier línea: seleccionar nota inicial, `Shift + clic` en nota final, clic en la línea de trino.

    Para cambiar el intervalo del trino (mayor, menor, aumentado, etc.), seleccionar el trino y usar los selectores de intervalo en el panel **Propiedades**. MuseScore mostrará la alteración correspondiente sobre el trino.


    ### Mordente

    El mordente es un adorno rápido de una sola alternancia:
    - **Mordente superior**: nota principal → nota superior → nota principal. Símbolo: `M` (línea quebrada sin tachar).
    - **Mordente inferior**: nota principal → nota inferior → nota principal. Símbolo: `M` con línea vertical que lo cruza.

    Se aplican seleccionando la nota y haciendo clic en el mordente correspondiente en la paleta **Ornamentos**. El intervalo (segunda mayor o menor) se configura en el panel **Propiedades**.


    ### Grupeto (turn)

    El grupeto ejecuta cuatro notas en secuencia: superior → principal → inferior → principal. La paleta **Ornamentos** ofrece:
    - **Grupeto normal**: comienza con la nota superior.
    - **Grupeto invertido**: comienza con la nota inferior.
    - **Grupeto entre notas**: se coloca entre dos notas; la primera nota se decora después de ser tocada.

    El intervalo superior e inferior se configuran individualmente en el panel **Propiedades**.

    ### Alteraciones en ornamentos

    Los ornamentos son conscientes de la armadura. Si un trino necesita una alteración que no está en la armadura —por ejemplo, un trino de tono sobre Fa en Do mayor necesita Fa♯— MuseScore muestra automáticamente la alteración necesaria.

    !!! warning "Las alteraciones de ornamento persisten en el compás"
        Si un ornamento introduce una alteración (ej. Sol♯ como auxiliar en un trino), MuseScore mantiene esa alteración para cualquier nota de ese mismo nombre que aparezca después en el MISMO compás. Esto es coherente con las reglas de notación tradicional.

    ### Propiedades de los ornamentos

    Desde el panel **Propiedades**, además del intervalo, se pueden ajustar:
    - **Visibilidad de alteraciones**: por defecto, solo se muestran las que no han aparecido antes en el compás. Se puede forzar "Mostrar cualquier alteración" o "Mostrar siempre".
    - **Colocación**: arriba o abajo.

???+ note "Ligaduras de expresión y de prolongación"

    Aunque visualmente ambas son líneas curvas, su función musical es completamente distinta:

    | Característica | Ligadura de expresión (slur) | Ligadura de prolongación (tie) |
    |---|---|---|
    | ¿Qué conecta? | Notas de **diferente** altura | Notas de la **misma** altura |
    | Función | Articulación *legato* | Extender la duración |
    | ¿Se articula la segunda nota? | Sí | **No** |
    | Atajo | `S` | `T` (modo ingreso) o `+` (modo normal) |

    ### Ligadura de expresión (slur)

    Para agregar una ligadura en **modo normal**:
    1. Seleccionar la primera nota de la frase.
    2. Presionar `S`. La ligadura se extiende hasta la nota siguiente.
    3. Para alargarla a más notas: mantener `Shift` + `→` repetidamente.
    4. Presionar `Esc` para salir del modo de edición.

    Para agregar una ligadura en **modo de ingreso** (`N`):
    1. Ingresar la primera nota.
    2. Presionar `S` (la ligadura comienza).
    3. Ingresar las notas restantes de la frase ligada.
    4. Presionar `S` de nuevo para cerrar la ligadura en la última nota.

    **Método 2 (selección con rango)**:
    1. Seleccionar la nota inicial.
    2. Mantener `Ctrl` (`Cmd` en macOS) y seleccionar la nota final.
    3. Presionar `S`. La ligadura cubrirá todas las notas en el rango.


    ### Ligaduras entre voces y entre pentagramas

    Usando el **Método 2** descrito arriba, se puede crear una ligadura entre notas de voces diferentes. Para mover manualmente el extremo de una ligadura entre voces, seleccionar el tirador de inicio o fin y usar `Shift + ↑` / `Shift + ↓`. Esto también permite crear ligaduras entre pentagramas (cross-staff).

    ### Ligadura de prolongación (tie)

    En **modo de ingreso**: ingresar la primera nota y presionar `T` inmediatamente después de la altura. La ligadura se crea y el cursor avanza listo para ingresar la segunda nota (que debe ser del mismo nombre).

    Para notas ya escritas en **modo normal**: seleccionar la primera nota y presionar `+`.


    ### Propiedades compartidas

    Seleccionando una ligadura, en el panel **Propiedades** se puede ajustar:
    - **Estilo**: sólida, guiones anchos, guiones finos o punteada.
    - **Posición**: arriba o abajo de las notas.

    Para la ligadura de prolongación, además: **Colocación de la ligadura** (extremos dentro o fuera de las cabezas de las notas).

    !!! tip "Ligadura vs. ligadura de prolongación: cómo no confundirlas"
        La regla es simple: si las notas son **iguales** y la segunda NO se articula, es ligadura de prolongación (`T` o `+`). Si las notas son **diferentes** y querés que suenen ligadas, es ligadura de expresión (`S`). La diferencia no es solo visual: en la reproducción, una ligadura de prolongación fusiona ambas notas en una sola duración continua.

---

## Actividad en Classroom

### Tarea: S09 — Articulaciones y ornamentos

> **Material necesario**: el docente proporcionará el archivo `ejercicio_S09_articulacion.mscz`, una partitura para instrumento de viento (flauta) en Sol mayor, 4/4, 20 compases con una melodía sin articulaciones ni ornamentos. Los compases 1–10 contienen la melodía base; los compases 11–20 están vacíos.

1. **Aplicar articulaciones a la melodía.** En los compases 1 a 10, agregá las siguientes articulaciones usando atajos de teclado:
    - Al menos 3 notas con **staccato** (`Shift + S`).
    - Al menos 3 notas con **tenuto** (`Shift + N`).
    - Al menos 2 notas con **acento** (`Shift + V`).
    - Al menos 2 notas con **marcato** (`Shift + O`).
    - Un **calderón** al final del compás 10 (sobre la última nota).
    - Probá combinaciones: al menos una nota con staccato + acento.

2. **Agregar ornamentos.** En los mismos compases 1 a 10:
    - Insertá un **trino** sobre una nota de cierta duración (negra o mayor). Probá con intervalo de tono (segunda mayor) y de semitono (segunda menor). ¿Se nota la diferencia auditiva?
    - Insertá un **mordente superior** y un **mordente inferior** en dos notas distintas.
    - Insertá un **grupeto** sobre una nota. Experimentá cambiando los intervalos superior e inferior en el panel Propiedades.

3. **Ligaduras de expresión.** En los compases 1 a 10:
    - Agrupá la melodía en frases de 2 a 4 notas usando ligaduras de expresión (`S` en modo normal o modo ingreso).
    - Usá al menos un **Método 2** (selección con `Ctrl + clic` en la nota final y luego `S`).
    - Ajustá al menos una ligadura manualmente arrastrando sus tiradores.

4. **Composición propia con articulaciones.** En los compases 11 a 20, creá tu propia melodía de 10 compases que incluya:
    - Las 5 articulaciones estudiadas (staccato, tenuto, acento, marcato, calderón).
    - Al menos 2 ornamentos diferentes.
    - Ligaduras de expresión definiendo frases claras.
    - Al menos una ligadura de prolongación (dos notas iguales unidas).
    - Verificá que el resultado suene expresivo y variado.

5. **Reproducción y escucha crítica.**
    - Reproducí toda la partitura con las articulaciones y ornamentos aplicados.
    - ¿El staccato realmente acorta las notas?
    - ¿El trino suena fluido?
    - ¿Las ligaduras de expresión logran el efecto *legato* esperado?
    - Ajustá cualquier articulación que no suene como esperabas.

### Entregables

- [ ] `APELLIDO_Nombre_S09_articulacion_v01.mscz` (partitura con todas las articulaciones y ornamentos)
- [ ] `APELLIDO_Nombre_S09_articulacion_v01.pdf`
- [ ] Captura de pantalla del compás 10 mostrando el calderón sobre la última nota
- [ ] Captura de pantalla de un trino con el panel de Propiedades visible (mostrando el intervalo configurado)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Articulaciones básicas | ≥3 staccato, ≥3 tenuto, ≥2 acento, ≥2 marcato correctamente aplicados con atajos | Faltan 1–2 tipos o algunos están en notas incorrectas | ≥3 tipos faltantes o mal aplicados |
| Calderón | Insertado al final del compás 10; la reproducción muestra la pausa | Insertado pero en nota incorrecta | No insertado |
| Ornamentos | Trino, mordente superior, mordente inferior y grupeto presentes y bien ubicados | 1–2 ornamentos ausentes | ≥3 ausentes o incorrectos |
| Ligadura de expresión | Frases correctamente ligadas; al menos un Método 2 usado; ≥2 frases definidas | Una frase ligada pero sin claridad | No usó ligaduras de expresión |
| Ligadura de prolongación | Al menos una ligadura de prolongación correctamente insertada entre notas del mismo nombre | Insertada pero entre notas diferentes | No insertada |
| Composición propia | Los 10 compases contienen todas las articulaciones y ornamentos requeridos; melódicamente coherente | Faltan 1–2 elementos en la composición | Composición muy incompleta o incoherente |
| Escucha crítica | Reprodujo, evaluó y ajustó las articulaciones según el resultado auditivo | Escuchó pero no ajustó | No reprodujo ni revisó |

---

*Basado en: MuseScore Studio 4 Handbook — Articulations, Ornaments, Slurs and ties | https://handbook.musescore.org*
