# Sesión 13: Repeticiones, voltas y saltos de navegación

📚 Handbook → Notation: Repeats and jumps, Voltas, Barlines | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="barra-repeticion"></a> **Barra de repetición (repeat barline)** | Barra de compás especial que indica que una sección debe repetirse. Se compone de una barra doble (fina + gruesa) con dos puntos. La barra de inicio de repetición tiene los puntos a la derecha; la de fin, a la izquierda. Ambas forman un "sándwich" de repetición. |
    | <a id="volta"></a> **Volta / Casilla (volta)** | Corchete horizontal con un número (1, 2, 3...) que se coloca sobre el final de una sección repetida. Indica finales alternativos: la primera vez se toca la casilla 1, se repite, y la segunda vez se salta a la casilla 2. En MuseScore, la volta se arrastra desde la paleta **Repeticiones y saltos**. |
    | <a id="dc"></a> **D.C. / Da Capo** | Significa "desde el principio". Indica que al llegar a esta marca, la ejecución debe volver al comienzo de la pieza y continuar hasta encontrar *Fine* o una doble barra final. |
    | <a id="ds"></a> **D.S. / Dal Segno** | Significa "desde el signo". Similar a D.C. pero en lugar de volver al principio, se vuelve a la marca de *segno* (𝄋). |
    | <a id="fine"></a> **Fine** | Marca que indica el final real de la pieza cuando se llega a ella durante una repetición por D.C. o D.S. No es una barra doble final: es la palabra "Fine" colocada sobre el compás donde realmente termina la ejecución. |
    | <a id="coda"></a> **Coda** | Sección final independiente de una pieza, separada del cuerpo principal. Se accede mediante el símbolo *To Coda* (a veces escrito como *Coda* dentro de un círculo o una mira 𝄌). La estructura típica es: cuerpo → D.S. → tocar hasta *To Coda* → saltar a la sección Coda al final. |
    | <a id="segno"></a> **Segno (signo 𝄋)** | Marca visual que se inserta en un compás concreto. Es el "punto de retorno" al que se vuelve cuando la partitura dice *D.S.* (Dal Segno). |
    | <a id="barra-compas"></a> **Barra de compás (barline)** | Línea vertical que separa los compases. MuseScore ofrece múltiples tipos: simple (normal), doble (cambio de sección), final (doble con barra gruesa), inicio de repetición, fin de repetición, y combinaciones (fin-inicio). |
    | <a id="salto-navegacion"></a> **Salto de navegación (jump)** | Término genérico para cualquier marca que modifica el orden de ejecución natural de izquierda a derecha: D.C., D.S., To Coda, Fine. El conjunto de estas marcas forma un "mapa de navegación" de la partitura. |
    | <a id="lista-repeticion"></a> **Lista de repetición (repeat list)** | En el panel Propiedades de una volta, la lista de repeticiones determina en qué pasadas se toca esa volta. Por defecto, la volta 1 se toca en la pasada 1, la volta 2 en la pasada 2, etc. Podés configurarlo para patrones más complejos (ej. `1,3` para primera y tercera vez). |

???+ note "Barras de repetición: el bloque fundamental"

    La repetición más básica en notación musical es la barra de repetición: un par de barras especiales que marcan el inicio y el fin de una sección que debe tocarse dos veces.

    ### Tipos de barras de repetición

    | Barra | Símbolo | Qué significa |
    |---|---|---|
    | **Inicio de repetición** | Doble barra con dos puntos **a la derecha** | Desde aquí empieza el bloque que se repite |
    | **Fin de repetición** | Doble barra con dos puntos **a la izquierda** | Hasta aquí llega el bloque; al llegar, volver al inicio de repetición (o al principio si no hay inicio explícito) |
    | **Fin-inicio** | Doble barra con puntos a AMBOS lados | La sección anterior termina su repetición Y la siguiente sección empieza su propia repetición. Dos en uno |

    ### Insertar una barra de repetición

    1. Seleccionar la barra de compás que querés cambiar.
    2. Abrir la paleta **Barras de compás** (o **Compases**).
    3. Arrastrar la barra de repetición sobre la barra existente, o hacer clic en la barra nueva.

    > Insertar captura de la paleta de Barras de compás mostrando las opciones: simple, doble, inicio de repetición, fin de repetición, fin-inicio, final.

    ### ¿Qué pasa si solo ponés el fin de repetición?

    Si colocás una barra de fin de repetición SIN una barra de inicio de repetición antes, MuseScore asume que la repetición empieza desde el principio de la pieza (o desde el inicio de repetición anterior más cercano). Es una práctica común en partituras sencillas.

    !!! tip "Repeticiones y reproducción"
        Cuando insertás barras de repetición correctamente y reproducís en MuseScore, el programa ejecuta la repetición automáticamente: toca la sección una vez, vuelve al inicio de repetición y la toca de nuevo. No tenés que hacer nada más. Si la repetición no se escucha, revisá que AMBAS barras (inicio y fin) estén insertadas.

    ### Anidar repeticiones

    Podés tener repeticiones dentro de repeticiones. Por ejemplo, una sección A que se repite, y dentro de ella una subsección que también se repite. MuseScore maneja esto correctamente en la reproducción siguiendo el orden lógico: repeticiones internas primero, luego las externas.

    > Insertar captura de una partitura con repeticiones anidadas: barra inicio-fin externa (c.1–16) y barra inicio-fin interna (c.5–8).

???+ note "Voltas: finales alternativos (primera y segunda vez)"

    Cuando una sección se repite pero el final cambia, usamos **voltas** (también llamadas casillas de repetición). El caso más común es "primera vez" y "segunda vez".

    ### Cómo funciona

    ```
    [ inicio de repetición ] ... compases comunes ... [ volta 1 ] :|| [ volta 2 ] ... resto ...
    ```

    La ejecución es:
    1. Tocar desde el inicio de repetición, pasando por los compases comunes.
    2. Entrar en la volta 1 y tocar hasta la barra de fin de repetición.
    3. Volver al inicio de repetición y tocar de nuevo los compases comunes.
    4. Esta vez, SALTAR la volta 1 y tocar directamente la volta 2.
    5. Continuar con el resto de la pieza.

    ### Insertar una volta

    1. Asegurate de que la barra de fin de repetición ya esté colocada.
    2. Seleccionar el compás o rango de compases que abarcará la volta.
    3. Ir a la paleta **Repeticiones y saltos** (o **Barlines** en versiones anteriores).
    4. Arrastrar la volta con el número deseado (1, 2, 3...) sobre el compás seleccionado.
    5. La volta se extiende automáticamente y queda anclada a la barra del compás.

    ### Ajustar la longitud de la volta

    Al seleccionar una volta, aparecen tiradores (cuadrados pequeños) en sus extremos. Arrastrá el tirador derecho para extender o acortar la volta sobre más o menos compases. La volta debe cubrir exactamente los compases que son diferentes en ese final alternativo.

    ### Configurar la lista de repetición

    Por defecto:
    - **Volta 1** se toca en la pasada 1 (y se salta en las siguientes).
    - **Volta 2** se toca en la pasada 2 (y se omite en las anteriores).

    Si necesitás un patrón más complejo (por ejemplo, una volta que se toque en las pasadas 1 y 3, pero no en la 2), seleccioná la volta y en el panel **Propiedades → Lista de repetición** escribí los números de pasada separados por comas: `1,3`.

    !!! warning "La volta y la barra de repetición deben coincidir"
        La volta 1 DEBE terminar con una barra de fin de repetición para que MuseScore entienda que ahí se repite. Si ponés la volta sobre una barra normal, MuseScore no repetirá y la volta no tendrá efecto.

    > Insertar captura de una partitura con volta 1 (2 compases, terminando en barra de fin de repetición) y volta 2 (2 compases, terminando en barra doble o simple), con la lista de repetición visible en el panel Propiedades.

???+ note "Saltos de navegación: D.C., D.S., Fine y Coda"

    Más allá de las repeticiones simples con barras, la notación musical tiene un sistema de "saltos" que modifican el orden de ejecución a gran escala. Son instrucciones como "volver al principio", "ir al signo", "saltar a la coda".

    ### D.C. al Fine (Da Capo al Fine)

    La estructura más común que combina salto y fin:

    ```
    [ inicio de la pieza ] ... música ... [ D.C. al Fine ] ... [ Fine ]
    ```

    Ejecución: tocar normalmente hasta encontrar *D.C. al Fine* → volver al principio → tocar de nuevo hasta encontrar *Fine* → terminar.

    ### D.S. al Fine (Dal Segno al Fine)

    Similar pero en lugar de volver al principio, se vuelve a la marca de *segno*:

    ```
    [ inicio ] ... [ 𝄋 segno ] ... música ... [ D.S. al Fine ] ... [ Fine ]
    ```

    Ejecución: tocar hasta *D.S. al Fine* → volver al *segno* → tocar desde ahí hasta encontrar *Fine*.

    ### D.S. al Coda

    La estructura más elaborada:

    ```
    [ inicio ] ... [ 𝄋 segno ] ... música ... [ To Coda 𝄌 ] ... [ D.S. al Coda ] ... [ 𝄌 Coda ]
    ```

    Ejecución:
    1. Tocar desde el principio normalmente.
    2. Al llegar a *D.S. al Coda*, volver al *segno*.
    3. Tocar desde el *segno* hasta encontrar *To Coda*.
    4. En *To Coda*, saltar a la sección *Coda* al final de la pieza.
    5. Tocar la Coda hasta el final.

    ### Insertar saltos en MuseScore

    Todos los saltos se encuentran en la paleta **Repeticiones y saltos**:

    1. Seleccionar el compás donde querés insertar el salto.
    2. Ir a la paleta **Repeticiones y saltos**.
    3. Arrastrar el salto deseado (D.C., D.S., Fine, To Coda, Coda) sobre la barra del compás o sobre el pentagrama en ese compás.

    !!! tip "Los saltos se arrastran sobre las BARRAS de compás"
        A diferencia de otros elementos que se colocan sobre notas, los saltos (D.C., D.S., Fine) suelen anclarse a la barra de compás. Seleccioná la barra o hacé clic en el compás y arrastrá el salto desde la paleta.

    ### Verificar la navegación

    MuseScore reproduce los saltos automáticamente. Para verificar que el "mapa de navegación" es correcto:
    1. Reproducir la pieza completa.
    2. Observar el cursor de reproducción: debe seguir el camino lógico de los saltos.
    3. Si la pieza se salta la Coda o no vuelve al segno, revisar que todos los elementos (segno, D.S., To Coda, Coda) estén correctamente anclados.

    > Insertar captura de la paleta Repeticiones y saltos mostrando D.C., D.S., Fine, To Coda, Coda, y Segno.

    !!! warning "No mezcles D.C. y D.S. sin necesidad"
        Si tenés una estructura D.C. al Fine, no pongas también un segno que no se usa. Cada salto debe tener un propósito claro en el mapa de navegación. Menos es más: una partitura con demasiadas marcas de navegación confunde al intérprete.

???+ note "Segno: la marca de retorno"

    El *segno* (𝄋) es simplemente una marca que dice "volvé acá cuando veas D.S.". No tiene efecto por sí mismo: necesita que exista un D.S. (Dal Segno) en algún punto posterior de la partitura.

    ### Insertar un segno

    1. Seleccionar el compás donde querés la marca.
    2. Ir a la paleta **Repeticiones y saltos**.
    3. Arrastrar el símbolo de *segno* sobre la barra del compás o sobre el primer tiempo del compás.
    4. El segno aparece sobre el pentagrama, típicamente alineado con la barra de compás.

    ### ¿Dónde se coloca?

    El segno se coloca al inicio del compás (sobre la barra izquierda) donde debe reanudarse la ejecución. La convención es que quede visible sobre el pentagrama, no dentro de él.

    > Insertar captura de un segno colocado sobre la barra de compás, con el resto de la partitura visible para contexto.

???+ note "Barras de compás especiales: más que simples líneas"

    Las barras de compás no son solo la línea vertical que separa un compás del siguiente. MuseScore ofrece varios tipos, cada uno con un significado musical.

    ### Tipos de barras y sus usos

    | Tipo | Apariencia | Cuándo usarla |
    |---|---|---|
    | **Simple** | Una línea fina | Separación normal entre compases. Es la predeterminada. |
    | **Doble** | Dos líneas finas | Cambio de sección, cambio de armadura, cambio de compás. Dice "acá empieza algo nuevo". |
    | **Final** | Línea fina + línea gruesa | Fin de la pieza o de un movimiento. La barra gruesa mira hacia afuera de la música. |
    | **Inicio de repetición** | Doble (fina+gruesa) + dos puntos a la derecha | Comienzo de sección que se repite. |
    | **Fin de repetición** | Doble (fina+gruesa) + dos puntos a la izquierda | Fin de sección que se repite. |
    | **Fin-inicio** | Puntos a ambos lados | Una sección termina su repetición y la siguiente empieza la suya. |
    | **Punteada** | Línea punteada | Raramente usada. Indica divisiones no estándar o compases de cortesía en ediciones modernas. |

    ### Cambiar el tipo de barra

    1. Seleccionar la barra de compás que querés cambiar.
    2. Ir a la paleta **Barras de compás**.
    3. Arrastrar el nuevo tipo de barra sobre la existente. MuseScore la reemplaza.

    O alternativamente:
    1. Seleccionar la barra.
    2. En el panel **Propiedades → Barra de compás**, elegir el tipo desde el desplegable.

    ### Doble barra vs. barra final

    Es un error común de principiante: poner una barra final en medio de la pieza para marcar un cambio de sección.

    - **Doble barra** = "cambio de sección, la pieza continúa".
    - **Barra final** = "acá se terminó, no hay más música".

    Si ponés una barra final en medio, MuseScore puede interpretar que la pieza terminó ahí y no reproducir lo que sigue. Usá barra doble para cambios de sección internos.

    > Insertar captura de la paleta de Barras de compás con todos los tipos desplegados y etiquetados.

---

## Actividad en Classroom

### Tarea: S13 — Repeticiones, voltas y saltos de navegación

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S13_repeticiones.mscz`, una partitura para piano en Do mayor, 4/4, 32 compases con una estructura A-B-A' donde la sección A (c.1–8) y B (c.9–16) deben repetirse, y un A' (c.17–32) que tiene dos finales alternativos; (b) `ejercicio_S13_navegacion.mscz`, una partitura para cuarteto de cuerdas (dos violines, viola, violonchelo) en Sol mayor, 3/4, 24 compases preparada para recibir una estructura D.S. al Coda; (c) `ejercicio_S13_barras.mscz`, una partitura para flauta sola en Fa mayor, 4/4, 16 compases con todas las barras de compás en tipo "simple" y errores de navegación intencionales.

1. **Barras de repetición y voltas en el piano.** Abrí `ejercicio_S13_repeticiones.mscz`:
    - Insertá las barras de **inicio de repetición** y **fin de repetición** en los compases 1–8 (sección A).
    - Insertá las barras de **inicio de repetición** y **fin de repetición** en los compases 9–16 (sección B).
    - En los compases 17–24 (primera parte de A'), colocá una **volta 1** que termine en barra de fin de repetición. Esta volta debe cubrir exactamente los compases 17–24.
    - En los compases 25–32 (segunda parte de A'), colocá una **volta 2** que termine con barra doble o final.
    - Reproducí la pieza completa. ¿Se escucha A-A-B-B-A'(volta1)-A-A-B-B-A'(volta2)?
    - Ajustá la lista de repetición de la volta 1 si es necesario.

2. **Navegación con D.S. al Coda en el cuarteto.** Abrí `ejercicio_S13_navegacion.mscz`:
    - La partitura tiene tres secciones claramente marcadas: Introducción (c.1–4), Tema (c.5–12), Desarrollo (c.13–24). Al final de la partitura hay 4 compases vacíos etiquetados como "Coda" (c.25–28).
    - Colocá un **segno** (𝄋) al inicio del Tema (compás 5).
    - Colocá un **To Coda** (𝄌) al final del Desarrollo (compás 24).
    - Colocá un **D.S. al Coda** al final del Tema, en el compás 12. Ajustá el diseño para que el D.S. quede visible.
    - La ruta de ejecución debe ser: Introducción → Tema (hasta D.S. al Coda) → volver al segno → Tema de nuevo → Desarrollo → To Coda → saltar a la sección Coda.
    - Reproducí y verificá que el orden de ejecución sea correcto.
    - Escribí en un comentario de Classroom el "mapa de navegación" con tus palabras: "La pieza empieza en ___, luego...".

3. **Corrección de barras de compás en la flauta.** Abrí `ejercicio_S13_barras.mscz`:
    - La partitura tiene TODAS las barras de compás como "simples", incluyendo el final. Corregí:
      - Colocá **doble barra** en los cambios de sección (indicados con texto "Sección B", "Sección C" sobre los compases correspondientes).
      - Reemplazá la última barra simple por una **barra final**.
      - Si hay secciones que claramente deberían repetirse según la estructura musical, insertá las barras de repetición correspondientes.
    - Documentá cada cambio en un comentario de Classroom: "Compás X: cambié barra simple por doble porque...".

4. **Diseño de mapa de navegación propio.** En el mismo archivo `ejercicio_S13_repeticiones.mscz` ya editado:
    - Al final de la pieza (después de la volta 2), agregá 8 compases nuevos (c.33–40) en ambos pentagramas del piano.
    - Componé una breve sección de cierre (Coda) de 8 compases.
    - Agregá un **segno** al inicio de la sección B (compás 9).
    - Modificá la estructura para que el orden de ejecución sea: A (con repetición) → B (con repetición) → A' (con voltas) → D.S. al Coda → B → Coda.
    - Ajustá todos los saltos necesarios: quitá el D.S. automático si sobra, agregá To Coda donde corresponda, verificá que el segno esté bien posicionado.
    - Reproducí la pieza completa. ¿Sigue el mapa de navegación que planeaste?

5. **Reflexión sobre navegación musical.** En Classroom, respondé:
    - ¿En qué se diferencia un D.C. de un D.S.? ¿Cuándo usarías uno y cuándo el otro?
    - ¿Por qué creés que existen las voltas en lugar de simplemente escribir la música dos veces? Mencioná al menos dos razones (pista: pensá en el papel, la tinta, y el trabajo del editor).
    - Si una partitura tiene un *Fine* pero no tiene ni D.C. ni D.S., ¿el *Fine* tiene algún efecto en la reproducción? Justificá tu respuesta.

### Entregables

- [ ] `APELLIDO_Nombre_S13_repeticiones_v01.mscz` (piano con repeticiones, voltas y Coda propia)
- [ ] `APELLIDO_Nombre_S13_repeticiones_v01.pdf`
- [ ] `APELLIDO_Nombre_S13_navegacion_v01.mscz` (cuarteto con D.S. al Coda funcional)
- [ ] `APELLIDO_Nombre_S13_navegacion_v01.pdf`
- [ ] `APELLIDO_Nombre_S13_barras_v01.mscz` (flauta con barras corregidas)
- [ ] `APELLIDO_Nombre_S13_barras_v01.pdf`
- [ ] Comentario en Classroom con: (a) mapa de navegación del cuarteto explicado con tus palabras, (b) lista de correcciones de barras (al menos 4 cambios documentados), (c) respuestas a las 3 preguntas de reflexión

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Barras de repetición (piano) | Inicio y fin correctos en A y B; las 4 barras insertadas y funcionales en reproducción | Repeticiones insertadas pero una sección no repite correctamente | Sin repeticiones o solo 1 sección |
| Voltas | Volta 1 y 2 correctamente posicionadas; volta 1 termina en repetición; la secuencia 1ª/2ª vez funciona | Voltas insertadas pero mal extendidas o sin barra de fin de repetición en volta 1 | Sin voltas o completamente incorrectas |
| D.S. al Coda (cuarteto) | Segno, To Coda, D.S. al Coda y Coda colocados; la navegación reproduce el orden correcto | Elementos colocados pero el orden de ejecución es incorrecto | Faltan elementos críticos o la navegación no funciona |
| Corrección de barras | Doble barra en ≥2 cambios de sección + barra final correcta; ≥4 cambios documentados | 2–3 cambios correctos o documentación incompleta | ≤1 cambio o sin documentación |
| Coda propia | 8 compases compuestos; segno reposicionado; D.S. al Coda funcional; mapa coherente | Coda compuesta pero la navegación falla en algún punto | Coda incompleta o navegación rota |
| Reflexión | Responde las 3 preguntas con claridad; demuestra comprensión conceptual | Responde 2 de 3 correctamente | No responde o las respuestas son incorrectas |

---

*Basado en: MuseScore Studio 4 Handbook — Repeats and jumps, Voltas, Barlines | https://handbook.musescore.org*
