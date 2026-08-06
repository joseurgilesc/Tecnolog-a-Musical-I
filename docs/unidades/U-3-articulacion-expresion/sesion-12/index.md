# Sesión 12: Escritura a múltiples voces

📚 Handbook → Basics: Working with multiple voices; Notation: Brackets | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="voz"></a> **Voz (voice)** | Línea melódica o rítmica independiente dentro de un mismo pentagrama. MuseScore permite hasta 4 voces por pentagrama, cada una con sus propias plicas, silencios y articulaciones. Se identifican con colores durante la edición. |
    | <a id="voz1"></a> **Voz 1 (azul)** | La voz principal y predeterminada. Todas las notas que ingresás sin especificar voz van a la Voz 1. Plicas hacia arriba por defecto. Color de edición: **azul**. |
    | <a id="voz2"></a> **Voz 2 (verde)** | Segunda voz. Por defecto, sus plicas van hacia abajo y sus silencios se posicionan en la parte baja del pentagrama. Color de edición: **verde**. |
    | <a id="voz3"></a> **Voz 3 (naranja)** | Tercera voz. Plicas hacia arriba, pero sus silencios y notas se desplazan para no colisionar con la Voz 1. Color de edición: **naranja**. |
    | <a id="voz4"></a> **Voz 4 (violeta)** | Cuarta voz. Plicas hacia abajo, con desplazamiento para no colisionar con la Voz 2. Color de edición: **violeta**. |
    | <a id="color-voces"></a> **Colores de voz (voice colors)** | Durante la edición, MuseScore colorea las cabezas de las notas según la voz a la que pertenecen para que puedas distinguirlas visualmente. Estos colores son solo para edición: no se imprimen ni se exportan. |
    | <a id="silencio-voz"></a> **Silencio de voz (voice rest)** | Cuando un compás tiene notas en una voz y silencios en otra, los silencios se muestran en diferentes posiciones verticales para cada voz. A veces es necesario ocultar silencios visualmente redundantes o moverlos manualmente. |
    | <a id="intercambio-voces"></a> **Intercambio de voces (voice exchange)** | Operación que intercambia el contenido de dos voces dentro de un rango seleccionado. Útil cuando necesitás que la melodía principal pase de la Voz 1 a la Voz 2 o viceversa. |
    | <a id="corchete"></a> **Corchete (bracket)** | Símbolo vertical que agrupa visualmente dos o más pentagramas pertenecientes a la misma familia instrumental o al mismo intérprete. Es puramente visual: NO afecta la reproducción. |
    | <a id="llave"></a> **Llave (brace / curly bracket)** | Símbolo curvo `{` que une pentagramas de un mismo instrumento. El caso más común es el gran pentagrama de piano: la llave conecta el pentagrama superior (mano derecha) con el inferior (mano izquierda). |
    | <a id="plica"></a> **Plica (stem)** | Línea vertical que sale de la cabeza de la nota. La dirección de la plica (arriba o abajo) depende de la posición de la nota en el pentagrama, pero en escritura a múltiples voces la dirección ayuda a distinguir visualmente cada voz. |
    | <a id="polifonia"></a> **Polifonía (polyphony)** | Textura musical en la que dos o más líneas melódicas independientes suenan simultáneamente. En notación, la polifonía se representa usando múltiples voces dentro del mismo pentagrama. |

???+ note "Voces en un pentagrama: concepto y activación"

    En música, es común que un mismo pentagrama contenga dos (o más) líneas independientes. Por ejemplo: una melodía y un bajo, dos líneas contrapuntísticas en un coral de Bach, o la separación entre manos en una pieza de guitarra.

    MuseScore resuelve esto con un sistema de **4 voces por pentagrama**.

    ### ¿Qué es una voz?

    Una voz es una "capa" independiente dentro de un pentagrama. Cada voz:
    - Tiene sus propias **notas y silencios**.
    - Tiene su propia **dirección de plicas** (arriba o abajo por defecto).
    - Mantiene sus propias **articulaciones y dinámicas** (aunque se pueden compartir si se configuran correctamente).
    - Se edita de forma independiente de las otras voces del mismo pentagrama.

    ### Identificación por colores

    Cuando estás editando una partitura con múltiples voces, las cabezas de las notas se muestran con colores para que puedas distinguir a qué voz pertenece cada una:

    | Voz | Color de edición | Dirección de plica por defecto | Uso típico |
    |---|---|---|---|
    | **Voz 1** | 🔵 Azul | Arriba | Melodía principal, línea superior |
    | **Voz 2** | 🟢 Verde | Abajo | Acompañamiento, contrapunto inferior |
    | **Voz 3** | 🟠 Naranja | Arriba | Tercera línea (uso avanzado) |
    | **Voz 4** | 🟣 Violeta | Abajo | Cuarta línea (uso avanzado) |

    !!! tip "Los colores de voz NO se imprimen"
        Los colores azul, verde, naranja y violeta son solo una ayuda visual durante la edición. En la vista normal, en el PDF exportado y en la impresión, todas las notas se ven en negro. Si los colores te distraen, podés desactivarlos en **Ver → Mostrar → Colores de voz**.

    ### Activar una voz para escribir

    Antes de MuseScore 4.4, el selector de voces estaba en la barra de herramientas de ingreso de notas (iconos `1`, `2`, `3`, `4`). En versiones recientes, está en la barra de herramientas de ingreso de notas en la parte superior:

    1. Activar el **modo de ingreso de notas** (`N`).
    2. Hacer clic en el número de voz deseado (1, 2, 3 o 4) en la barra de herramientas.
    3. Ingresar las notas normalmente. Todas las notas ingresadas pertenecerán a la voz seleccionada.

    > Insertar captura de la barra de herramientas de ingreso de notas mostrando los botones de selección de voz 1–4 resaltados.

    ### Cambiar la voz de notas ya escritas

    Si ya escribiste notas en una voz equivocada:
    1. Seleccionar el rango de notas que querés cambiar.
    2. Ir al menú **Herramientas → Voces** y elegir la voz de destino.
    3. O usar el atajo `Ctrl + Alt + 1` (para Voz 1), `Ctrl + Alt + 2` (para Voz 2), etc. (`Cmd` en macOS).

???+ note "Escritura a dos voces: Voz 1 y Voz 2"

    El caso más común de polifonía es escribir **dos líneas independientes** en un mismo pentagrama. Vamos paso a paso.

    ### Paso 1: Escribir la Voz 1 (melodía superior)

    1. Activar modo de ingreso (`N`).
    2. Asegurarse de que la **Voz 1** esté seleccionada (botón `1` activo).
    3. Ingresar la melodía principal normalmente.

    ### Paso 2: Escribir la Voz 2 (línea inferior)

    1. Volver al inicio del pasaje (`Ctrl + Inicio` o `Cmd + Inicio`).
    2. Asegurarse de que la **Voz 2** esté seleccionada (botón `2` activo).
    3. Ingresar la línea inferior. Notarás que:
       - Las cabezas de las notas son de color **verde** durante la edición.
       - Las plicas van hacia **abajo** por defecto.
       - Los silencios se colocan en la parte **baja** del pentagrama.
    4. Donde la Voz 2 tenga silencio pero la Voz 1 tenga nota, MuseScore inserta automáticamente silencios ocultos o visibles según el contexto.

    > Insertar captura de un pentagrama con Voz 1 (azul, plicas arriba) y Voz 2 (verde, plicas abajo) visibles simultáneamente, con algunas notas en una voz y silencios en la otra.

    ### Regla de duraciones completas

    Cada voz debe completar las duraciones del compás de forma independiente. Si un compás es 4/4:
    - La Voz 1 debe sumar 4 tiempos (con notas y silencios).
    - La Voz 2 debe sumar 4 tiempos (con notas y silencios), aunque visualmente algunos silencios de la Voz 2 puedan ocultarse si hay notas de la Voz 1 en esos tiempos.

    ### Dirección de plicas

    Por defecto:
    - **Voz 1**: plicas hacia **arriba**.
    - **Voz 2**: plicas hacia **abajo**.

    Esto no es una regla rígida. Si trabajás con más de 2 voces o la lógica musical lo requiere, podés forzar la dirección de la plica seleccionando una nota y usando el panel **Propiedades → Dirección de la plica**.

???+ note "Voces 3 y 4: cuándo y cómo usarlas"

    Para la mayoría de situaciones, dos voces (1 y 2) son suficientes. Las voces 3 y 4 se reservan para casos específicos.

    ### ¿Cuándo necesitás 3 o 4 voces?

    Situaciones típicas:
    - **Coral a 4 partes en un pentagrama**: aunque lo más común es usar dos pentagramas (soprano/alto y tenor/bajo), a veces se escribe todo en uno.
    - **Acordes con ritmos independientes**: si tenés un acorde de 3 notas donde cada nota tiene un ritmo diferente, necesitás una voz por cada ritmo.
    - **Percusión en pentagrama de 5 líneas**: cada elemento del set (bombo, caja, hi-hat) puede ocupar una voz distinta.
    - **Pasajes de contrapunto denso** donde 2 voces no alcanzan para diferenciar las líneas melódicas.

    ### Cómo trabajar con Voz 3 y Voz 4

    | Voz | Color | Plica por defecto | Posición de silencios |
    |---|---|---|---|
    | **Voz 3** | Naranja | Arriba | Se desplaza para no colisionar con Voz 1 |
    | **Voz 4** | Violeta | Abajo | Se desplaza para no colisionar con Voz 2 |

    El proceso de ingreso es el mismo: seleccionar la voz en la barra de herramientas y escribir. Sin embargo, a medida que agregás más voces, la partitura se vuelve más densa y requiere más ajustes manuales.

    ### Ocultar silencios innecesarios

    Cuando usás 3 o 4 voces, muchos silencios se vuelven visualmente redundantes. Para ocultarlos:
    1. Seleccionar el silencio.
    2. Presionar `V` (atajo de visibilidad). El silencio se vuelve gris (oculto en la vista final, pero sigue existiendo).
    3. O desde el panel **Propiedades → Visible**, desmarcar la casilla.

    > Insertar captura de un pentagrama con 3 voces activas en un compás denso: Voz 1 (azul), Voz 2 (verde), Voz 3 (naranja), mostrando un silencio oculto en gris.

    !!! warning "No abuses de las voces 3 y 4"
        Antes de usar la Voz 3, preguntate: ¿esto se podría resolver con dos voces y mejor distribución de plicas? ¿Sería más legible dividir el contenido en dos pentagramas? En notación profesional, rara vez se usan más de 2 voces en un pentagrama, excepto en contextos muy específicos como percusión o contrapunto denso.

???+ note "Herramientas de gestión de voces"

    MuseScore incluye varias herramientas para manipular voces después de haber escrito las notas.

    ### Intercambiar voces

    Si escribiste la melodía en Voz 1 y el acompañamiento en Voz 2, pero querés intercambiarlas:

    1. Seleccionar el rango de compases donde están ambas voces.
    2. Ir a **Herramientas → Voces → Intercambiar voz 1 y voz 2**.
    3. El contenido de ambas voces se intercambia manteniendo las plicas y posiciones.

    **Variantes disponibles:**
    - Intercambiar voz 1 ↔ 2
    - Intercambiar voz 1 ↔ 3
    - Intercambiar voz 1 ↔ 4
    - Intercambiar voz 2 ↔ 3
    - Intercambiar voz 2 ↔ 4
    - Intercambiar voz 3 ↔ 4

    ### Mover notas a otra voz

    Si necesitás mover solo ALGUNAS notas (no todo el contenido) de una voz a otra:
    1. Seleccionar las notas que querés mover.
    2. Ir a **Herramientas → Voces → Mover a voz 2** (o la voz de destino).
    3. O usar los atajos: `Ctrl + Alt + 1` para Voz 1, `Ctrl + Alt + 2` para Voz 2, etc.

    Si la voz de destino ya tiene contenido en el mismo tiempo, MuseScore puede fusionar las notas o generar un conflicto. Es recomendable hacerlo por compases separados y revisar cada uno.

    ### Separar voces en pentagramas distintos

    Si escribiste una partitura con dos voces en un pentagrama y luego decidís que sería mejor separarlas en dos pentagramas independientes:

    1. Seleccionar el rango completo.
    2. Ir a **Herramientas → Voces → Separar en pentagramas** (o similar, según la versión).
    3. MuseScore extrae la Voz 1 a un pentagrama y la Voz 2 a otro.

    La funcionalidad exacta puede variar según la versión. En versiones recientes, se encuentra en **Herramientas → Explotar** (*Explode*), que separa el contenido de un pentagrama en varios pentagramas según las voces.

    > Insertar captura del menú Herramientas → Voces mostrando las opciones de intercambio, movimiento y separación.

    ### Silencios por voz: visibilidad y ocultamiento

    Una de las tareas más frecuentes al trabajar con voces es manejar los silencios:

    - **Silencio visible**: aparece cuando una voz tiene ausencia total de sonido en un tiempo. Se posiciona según la voz (Voz 1: alto, Voz 2: bajo, etc.).
    - **Silencio oculto**: se puede ocultar seleccionándolo y presionando `V`. Útil cuando otra voz ya "cubre" ese tiempo y el silencio es redundante.
    - **Ocultamiento automático**: en pasajes a dos voces, MuseScore oculta automáticamente algunos silencios redundantes. Si no lo hace, podés forzar la visibilidad desde el panel Propiedades.

    !!! tip "Regla de oro de los silencios en voces"
        Si la otra voz tiene una nota en el mismo tiempo, el silencio de esta voz probablemente sobra. Si ambas voces están en silencio en ese tiempo, debe mostrarse al menos un silencio (normalmente en la voz con el número más bajo) para que el compás "cuadre" visualmente.

???+ note "Corchetes y llaves: agrupación de pentagramas"

    Aunque no son parte directa de la escritura a voces, los corchetes y llaves organizan visualmente los pentagramas de una partitura. Son fundamentales para que un ensamble se vea profesional.

    ### Tipos de agrupación

    | Símbolo | Nombre | Uso | ¿Afecta reproducción? |
    |---|---|---|---|
    | `[` | **Corchete recto** (bracket) | Agrupa instrumentos de la misma familia (ej. todos los violines, todos los vientos). NO conecta las barras de compás. | No (visual) |
    | `{` | **Llave** (brace) | Une pentagramas de un MISMO instrumento (ej. piano, arpa). Conecta las barras de compás formando el "gran pentagrama". | No (visual) |
    | Línea de compás extendida | **Barra de compás común** | Las barras de compás atraviesan los pentagramas agrupados, dando unidad visual. | No (visual) |

    ### Insertar o modificar corchetes y llaves

    Los corchetes y llaves se configuran desde el panel de **Instrumentos** o desde el diálogo **Editar instrumento**:

    1. Abrir la paleta **Instrumentos** (`I`).
    2. Seleccionar el instrumento o grupo de pentagramas.
    3. Usar los controles de **Corchete** y **Llave** en el panel.

    O desde la partitura directamente:
    1. Seleccionar un pentagrama.
    2. Ir a **Formato → Estilo → Pentagramas** (o **Partes**).
    3. Configurar la agrupación de corchetes y llaves para cada sección de la partitura.

    > Insertar captura del panel de Instrumentos mostrando un ensamble mixto con corchetes para la familia de cuerdas y vientos, y llave para los dos pentagramas del piano.

    ### Corchetes y llaves en el contexto de este curso

    En las sesiones anteriores ya trabajaste con ensambles que tenían corchetes (cuarteto de cuerdas, cuarteto de vientos). MuseScore los crea automáticamente al seleccionar la plantilla del ensamble.

    Lo importante para esta sesión es que comprendas que los corchetes y llaves son puramente **visuales**: no afectan la reproducción y no tienen relación con las voces dentro de un pentagrama. Son dos conceptos distintos:
    - **Voces**: capas melódicas DENTRO de un pentagrama (1, 2, 3, 4).
    - **Corchetes/llaves**: agrupación visual ENTRE pentagramas.

    !!! tip "Voces vs. pentagramas: elegir la herramienta correcta"
        Cuando tenés dos líneas musicales, la decisión de diseño es: ¿las escribo en dos voces de un mismo pentagrama, o en dos pentagramas separados? La respuesta depende del contexto instrumental y de la claridad de lectura:
        - **En un mismo pentagrama con 2 voces**: si ambas líneas pertenecen al MISMO instrumento y tienen un ámbito compartido (ej. dos líneas en una guitarra, contrapunto en un teclado, dos partes vocales en un pentagrama de ensayo).
        - **En pentagramas separados**: si corresponden a instrumentos distintos (ej. violín I y violín II) o si la densidad de cada línea justifica su propio espacio (ej. mano derecha e izquierda del piano).

---

## Actividad en Classroom

### Tarea: S12 — Escritura a múltiples voces

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S12_voces.mscz`, una partitura para piano (gran pentagrama) en Do mayor, 4/4, 16 compases donde el pentagrama superior contiene una melodía monofónica en Voz 1 (compases 1–8) y el pentagrama inferior contiene un bajo simple (compases 1–8) — los compases 9–16 están vacíos en ambos pentagramas; (b) `ejercicio_S12_coral.mscz`, una partitura para voz (un solo pentagrama) en Fa mayor, 3/4, 8 compases con la melodía de un coral en Voz 1, preparado para añadir una segunda voz; (c) `ejercicio_S12_limpieza.mscz`, una partitura para guitarra (un pentagrama) en La menor, 4/4, 12 compases con errores intencionales de voces: silencios innecesarios, colisiones visuales, dirección de plicas inconsistente y al menos 8 notas en la voz equivocada.

1. **Escritura a dos voces en pentagrama superior del piano.** Abrí `ejercicio_S12_voces.mscz`:
    - Los compases 1–8 del pentagrama superior (mano derecha) tienen una melodía en Voz 1. Agregá una **segunda voz** (Voz 2) debajo de esa melodía, a distancia de tercera o sexta, creando un paralelismo armónico.
    - Asegurate de que la Voz 2 complete las duraciones de cada compás (notas + silencios).
    - Comprobá que las plicas de la Voz 2 apunten hacia abajo y no colisionen con la Voz 1.
    - Donde haya silencios redundantes en Voz 2 (porque Voz 1 tiene nota), ocultalos seleccionándolos y presionando `V`.

2. **Escritura a dos voces en pentagrama inferior del piano.** En el mismo archivo:
    - Los compases 1–8 del pentagrama inferior (mano izquierda) tienen un bajo simple en Voz 1. Agregá una **segunda voz** (Voz 2) por encima de ese bajo, creando un acompañamiento rítmico de acordes quebrados o notas repetidas.
    - La Voz 2 debe tener un ritmo diferente al bajo de Voz 1 (ej. corcheas regulares contra blancas del bajo).
    - Verificá la dirección de plicas: Voz 1 (bajo, abajo), Voz 2 (acompañamiento, arriba).
    - Ocultá los silencios redundantes.

3. **Composición a dos voces.** En los compases 9–16 de ambos pentagramas del piano:
    - En el pentagrama superior, componé una nueva frase de 8 compases a **dos voces** totalmente original.
    - En el pentagrama inferior, componé un acompañamiento también a **dos voces**.
    - La textura resultante debe ser polifónica: no se trata de acordes (todas las voces con el mismo ritmo), sino de líneas con cierta independencia rítmica y melódica.
    - Verificá que los 8 compases en TODAS las voces estén completos en duraciones.

4. **Añadir segunda voz a un coral.** Abrí `ejercicio_S12_coral.mscz`:
    - La partitura contiene la melodía de un coral en Voz 1. Agregá una **Voz 2** que funcione como contrapunto, creando intervalos consonantes (terceras, sextas) con algunas notas de paso y movimiento contrario ocasional.
    - Prestá especial atención a:
      - Que las plicas de Voz 2 vayan hacia abajo.
      - Que los silencios de Voz 2 sean mínimos (siempre que sea posible, que la Voz 2 tenga nota).
      - Que no haya colisiones entre las cabezas de las notas (si dos voces comparten la misma altura, MuseScore las superpone automáticamente con cabezas desplazadas).
    - Reproducí el resultado: ¿se distinguen las dos líneas melódicas auditivamente?

5. **Limpieza y corrección de voces.** Abrí `ejercicio_S12_limpieza.mscz`:
    - Revisá cada compás y detectá los problemas:
      - Notas en la voz equivocada (melodía que debería estar en Voz 1 está en Voz 2, o viceversa).
      - Silencios visibles innecesarios que deberían ocultarse.
      - Colisiones visuales: notas demasiado juntas o plicas que chocan con cabezas de la otra voz.
      - Dirección de plicas inconsistente (Voz 1 con plicas hacia abajo, Voz 2 con plicas hacia arriba, cuando debería ser al revés).
    - Corregí cada error y documentá los cambios en un comentario de Classroom: "Compás X: moví las notas de Voz 2 a Voz 1 porque...", "Compás Y: oculté silencio porque...".

6. **Reflexión sobre corchetes y llaves.** En el archivo `ejercicio_S12_voces.mscz` ya corregido:
    - Observá cómo están agrupados los dos pentagramas del piano (llave `{` + barra de compás común).
    - En Classroom, respondé brevemente: ¿por qué los dos pentagramas del piano llevan llave y no corchete? ¿Qué pasaría si un cuarteto de cuerdas tuviera llave en vez de corchete? ¿Cambiaría la reproducción?

### Entregables

- [ ] `APELLIDO_Nombre_S12_voces_v01.mscz` (piano completo con dos voces en ambos pentagramas, compases 1–8 editados y 9–16 originales)
- [ ] `APELLIDO_Nombre_S12_voces_v01.pdf`
- [ ] `APELLIDO_Nombre_S12_coral_v01.mscz` (coral a dos voces)
- [ ] `APELLIDO_Nombre_S12_coral_v01.pdf`
- [ ] `APELLIDO_Nombre_S12_limpieza_v01.mscz` (versión corregida con todos los errores resueltos)
- [ ] `APELLIDO_Nombre_S12_limpieza_v01.pdf`
- [ ] Comentario en Classroom con: (a) lista de correcciones del ejercicio de limpieza (al menos 8 correcciones documentadas), (b) respuesta a las preguntas sobre corchetes y llaves

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Dos voces en pentagrama superior | Voz 2 añadida con paralelismo correcto; plicas hacia abajo; silencios redundantes ocultos | Voz 2 añadida pero con plicas incorrectas o silencios sin ocultar | Sin segunda voz o llena de errores |
| Dos voces en pentagrama inferior | Voz 2 añadida con ritmo independiente; plicas hacia arriba; silencios ocultos correctamente | Voz 2 presente pero sin independencia rítmica o con plicas invertidas | Sin segunda voz en el bajo |
| Composición a dos voces (c.9–16) | Ambos pentagramas con dos voces originales; ritmo independiente entre voces y manos | Solo un pentagrama con dos voces o poca independencia | Composición incompleta o solo monofónica |
| Coral a dos voces | Voz 2 contrapuntística añadida; plicas, silencios y colisiones gestionados | Voz 2 añadida pero con colisiones o silencios problemáticos | Sin Voz 2 o con errores graves de notación |
| Limpieza de voces | 8 o más errores identificados y corregidos correctamente; documentación clara | 5–7 errores corregidos o documentación incompleta | <5 errores corregidos o sin documentación |
| Corchetes y llaves | Responde correctamente las preguntas; comprende la diferencia conceptual | Responde parcialmente (1 de 2 preguntas correcta) | No responde o responde incorrectamente |

---

*Basado en: MuseScore Studio 4 Handbook — Working with multiple voices, Brackets | https://handbook.musescore.org*
