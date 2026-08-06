# Sesión 26: Formato de página y disposición

📚 Handbook → Formatting: Page settings, Layout and formatting, Breaks and spacers | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="page-settings"></a> **Configuración de página (Page settings)** | Conjunto de parámetros que definen las dimensiones físicas y la escala de la partitura: tamaño de papel (A4, Carta, Oficio, Tabloide), orientación (vertical/retrato u horizontal/apaisado), márgenes (superior, inferior, izquierdo, derecho) y factor de escala general. Accesible desde **Formato → Configuración de página**. Es el PRIMER paso antes de formatear cualquier partitura seria. |
    | <a id="staff-space"></a> **Espacio de pentagrama (Staff space / sp)** | Unidad de medida fundamental en notación musical digital. 1 sp = la distancia entre dos líneas del pentagrama. TODAS las demás medidas (tamaño de notas, distancia entre sistemas, márgenes, grosor de líneas) se expresan en sp. Cambiar el staff space escala TODA la partitura proporcionalmente. Por defecto: 1.750 mm en MuseScore. |
    | <a id="scaling"></a> **Escala (Scaling)** | Factor que multiplica el staff space para adaptar el tamaño de la partitura al formato de papel deseado sin cambiar las proporciones internas. Si la partitura no entra en la página, NO cambies los márgenes: reducí la escala (ej. de 1.750 mm a 1.600 mm). Si sobra espacio, aumentala. La escala correcta se determina por PRUEBA Y ERROR visual. |
    | <a id="layout-formatting"></a> **Formato y disposición (Layout and formatting)** | Proceso de ajustar cómo se distribuyen los pentagramas, sistemas y compases en cada página. Incluye: número de compases por sistema, distancia entre pentagramas, espacio entre sistemas, justificación de compases y estiramiento horizontal. Es la diferencia entre una partitura "apiñada e ilegible" y una "profesional y cómoda de leer". |
    | <a id="system-break"></a> **Salto de sistema (System break)** | Marca que fuerza a MuseScore a comenzar un NUEVO SISTEMA (conjunto de pentagramas que se leen simultáneamente) en ese punto exacto. El sistema actual se corta aunque no esté lleno. Se inserta seleccionando un compás y usando el atajo `Enter` (sistema) o desde la paleta **Saltos y espaciadores**. |
    | <a id="page-break"></a> **Salto de página (Page break)** | Marca que fuerza a MuseScore a comenzar una NUEVA PÁGINA en ese punto exacto. La página actual se corta aunque tenga espacio disponible. Se inserta con `Ctrl + Enter` o desde la paleta. Esencial para controlar exactamente qué compases aparecen en cada página. |
    | <a id="section-break"></a> **Salto de sección (Section break)** | Tipo especial de salto que, además de comenzar un nuevo sistema o página, reinicia ciertas propiedades musicales: numeración de compases, armadura de cortesía, doble barra. Se usa para separar movimientos dentro de una misma obra (I. Allegro, II. Adagio) o para cambios estructurales importantes. |
    | <a id="spacer"></a> **Espaciador (Spacer)** | Elemento de formato que modifica la distancia vertical u horizontal entre pentagramas o sistemas sin insertar un salto. Hay dos tipos: (1) **espaciador de pentagrama** (arrastra hacia abajo/arriba un pentagrama individual), (2) **espaciador de sistema** (aumenta/reduce la distancia entre sistemas). Se insertan desde la paleta **Saltos y espaciadores**. Son la herramienta FINA para ajustar la aeración visual de la partitura. |
    | <a id="justification"></a> **Justificación (Justify)** | Proceso por el cual los compases de un sistema se estiran para ocupar TODO el ancho disponible entre los márgenes izquierdo y derecho, al igual que un texto justificado. MuseScore justifica el ÚLTIMO sistema de la partitura por defecto, pero los sistemas intermedios normalmente NO se justifican (quedan "alineados a la izquierda"). El ancho de cada compás se determina por su contenido rítmico: un compás de redondas es más angosto que uno de semicorcheas. |
    | <a id="page-fill"></a> **Relleno de página (Page fill)** | Umbral que determina cuánto debe "llenarse" el último sistema de una página para que MuseScore lo considere completo y pase al siguiente. Si el último sistema de la página tiene menos compases que el umbral, MuseScore "estira" los compases anteriores para ocupar el espacio. Se configura en **Formato → Estilo → Página → Umbral de relleno de página**. |
    | <a id="min-system-distance"></a> **Distancia mínima de sistema** | Espacio vertical mínimo entre el último pentagrama del sistema superior y el primer pentagrama del sistema inferior. Si se reduce demasiado, los sistemas se "pegan" y las indicaciones de tempo, dinámicas o matices del sistema superior invaden el sistema de abajo. Si es demasiado grande, se desperdicia espacio vertical. |
    | <a id="stretch"></a> **Estiramiento (Stretch)** | Factor que controla el ancho horizontal de un compás individual. 1.0 = ancho automático basado en el contenido. >1.0 = más ancho. <1.0 = más angosto. Se ajusta seleccionando el compás y usando las flechas en la paleta **Propiedades de compás** o `Alt + ← / →`. El estiramiento es el "ajuste fino" para cuando la justificación automática no convence. |
    | <a id="vertical-spacing"></a> **Espaciado vertical** | Conjunto de parámetros que controlan la distancia entre elementos verticales: pentagramas de un mismo sistema, sistemas consecutivos, pentagramas y líneas de texto, pentagramas y dinámicas. Un mal espaciado vertical es la causa #1 de partituras que parecen "amateur": pentagramas amontonados, matices que chocan con el pentagrama de abajo, indicaciones de tempo que tapan las notas. |

???+ note "La partitura como objeto físico: página, margen y escala"

    Una partitura NO es un archivo digital. Es un OBJETO FÍSICO que alguien va a imprimir, poner en un atril y leer a cierta distancia. Todo el formateo de página existe para servir a ese momento: el músico frente al atril.

    ### El triángulo del formato de página

    Tres variables interdependientes que definen cómo se ve tu partitura impresa:

    | Variable | ¿Qué controla? | Pregunta clave |
    |---|---|---|
    | **Tamaño de papel** | Dimensiones físicas (A4 = 210×297 mm, Carta = 215.9×279.4 mm, Tabloide = 279.4×431.8 mm) | ¿En qué papel se va a imprimir? |
    | **Márgenes** | Espacio en blanco alrededor de la música (superior, inferior, izquierdo, derecho) | ¿Cuánto espacio necesita el atril? ¿Hay que encuadernar? |
    | **Escala (scaling)** | Tamaño visual de las notas y pentagramas (staff space en mm) | ¿A qué distancia va a leer el músico? |

    ### La regla de los formatos estándar

    | Formato | Tamaño | ¿Cuándo usarlo? |
    |---|---|---|
    | **A4 vertical** | 210×297 mm | Partitura de piano, canción, ejercicio, estudio, partitura individual |
    | **A4 horizontal** | 297×210 mm | Música de cámara, ensamble pequeño (2–8 instrumentos) |
    | **Carta (Letter)** | 215.9×279.4 mm | Estándar en Estados Unidos y Latinoamérica. Mismas aplicaciones que A4. |
    | **Tabloide / A3** | 279.4×431.8 mm / 297×420 mm | Partitura de orquesta, banda sinfónica, ensamble grande (10+ pentagramas). El director necesita ver muchos pentagramas simultáneamente. |
    | **A5** | 148×210 mm | Partitura de bolsillo (estudio), edición económica, coro de pocas voces. |

    !!! tip "La distancia del atril determina la escala"
        Un pianista lee a ~50 cm del atril → staff space de 1.750 mm (default) está bien.  
        Un director de orquesta lee a ~80–100 cm del atril → necesita staff space de 1.500–1.600 mm para que todo entre en la página pero que sea LEGIBLE.  
        Un violinista en un foso de teatro lee a ~40 cm → staff space de 1.750 mm o más.  
        Moraleja: la escala NO es un capricho estético. Es ERGONOMÍA VISUAL.

    ### Configuración de página paso a paso

    1. **Formato → Configuración de página**.
    2. **Tamaño de papel**: seleccionar A4, Carta u otro según el estándar local.
    3. **Orientación**: vertical para pocos pentagramas (piano solo), horizontal para ensambles.
    4. **Márgenes**:
        - **Izquierdo** ligeramente mayor que el derecho si se va a encuadernar o anillar (15–20 mm en lugar de 10–12 mm).
        - **Superior e inferior**: simétricos (12–15 mm).
        - Si la partitura va en un atril que "muerde" la parte inferior, aumentar el margen inferior a 20–25 mm para que el atril no tape las notas.
    5. **Espacio de pentagrama (staff space)**: por defecto 1.750 mm. Reducir si la partitura no entra, aumentar si sobra espacio.
    6. **Aplicar** y revisar visualmente: todas las páginas deben verse proporcionadas.

    !!! warning "No cambies la escala para 'hacer que entre'. Ese es el camino del amateur."
        Si tu partitura no entra en la página, tenés 3 opciones, en este orden: (1) ajustar saltos de sistema para distribuir mejor los compases, (b) reducir la cantidad de compases por sistema, (c) reducir la escala como ÚLTIMO recurso. El amateur reduce la escala a ciegas y termina con una partitura microscópica ilegible. El profesional primero agota las opciones de formato.

    > Insertar captura del diálogo de Configuración de página mostrando las pestañas de Tamaño de papel, Márgenes y las opciones de escala.

???+ note "Diseño y distribución: cómo respira la partitura"

    Una partitura bien formateada "respira". Hay espacio entre pentagramas, entre sistemas, entre compases. El ojo del músico se mueve fluidamente sin chocar con otros elementos. Una partitura mal formateada es como un texto sin separación entre párrafos: se puede leer, pero cuesta el triple.

    ### La distancia entre pentagramas: el oxígeno de la partitura

    Los pentagramas de un MISMO sistema están separados por la **distancia de pentagrama** (ajustable en **Formato → Estilo → Página**). Los sistemas consecutivos están separados por la **distancia de sistema**. La regla de oro es:

    > **Distancia de sistema ≥ Distancia de pentagrama × 2**

    Si la distancia entre sistemas es igual o menor que la distancia entre pentagramas, el ojo no sabe dónde termina un sistema y empieza el siguiente. Es como escribir sin punto y aparte.

    ### Cuándo y cómo ajustar el layout

    | Síntoma | Diagnóstico | Solución |
    |---|---|---|
    | La última página tiene solo 2 compases (página casi vacía) | Mala distribución de compases entre páginas | Insertar saltos de página para redistribuir compases entre las páginas anteriores |
    | Hay compases con notas "aplastadas" (semicorcheas ilegibles) | Compás demasiado angosto para su contenido rítmico | Aumentar el estiramiento (`Alt + →`), o reducir la cantidad de compases por sistema |
    | Hay compases con mucho espacio vacío (una redonda ocupa media página) | Compás demasiado ancho para su contenido | Reducir estiramiento (`Alt + ←`), o aumentar la cantidad de compases por sistema |
    | Dinámicas del pentagrama superior invaden el pentagrama inferior | Distancia entre pentagramas insuficiente | Aumentar la distancia de pentagrama, o mover las dinámicas hacia arriba |
    | El último sistema de la página está "corto" (no llega al margen derecho) | Umbral de relleno de página muy alto (por defecto 70%) | Reducir el umbral en **Estilo → Página → Umbral de relleno**, o ajustar manualmente con estiramiento |
    | Indicaciones de tempo tapan el primer pentagrama | La distancia entre el margen superior y el primer pentagrama es insuficiente | Aumentar el margen superior, o mover la indicación de tempo más arriba |

    ### La mentalidad del formateador profesional

    El formateo de partituras NO es un proceso de "poner bonito". Es un proceso de TOMA DE DECISIONES. Cada página, cada sistema, cada compás es una decisión:

    1. **¿Este salto de página corta una frase musical?** Si la respuesta es sí, el salto está mal puesto. Los músicos respiran entre frases, no en el medio. El salto de página debe coincidir con finales de frase, dobles barras o calderones.
    2. **¿El músico puede pasar la página sin perder el ritmo?** En una partitura de orquesta, el pasaje de página debe ocurrir durante un silencio largo del instrumento. Si el músico está tocando semicorcheas cuando tiene que pasar la página, armaste un problema.
    3. **¿Cada sistema tiene sentido musical?** Un sistema NO debería empezar o terminar en medio de una ligadura de expresión o un regulador (crescendo/diminuendo). Si pasa, ajustá los saltos.
    4. **¿La página se ve equilibrada?** Los pentagramas no deberían estar todos en la mitad superior de la página con la mitad inferior vacía (ni viceversa). Si pasa, ajustá la distancia entre sistemas o usá espaciadores.

    > Insertar captura de "antes y después": una misma partitura con formato automático de MuseScore (default) y la misma partitura con formato manual profesional (saltos de página, espaciadores, estiramientos ajustados).

???+ note "Saltos de sistema, página y sección: tomando el control"

    MuseScore hace un formato automático decente. Pero "decente" NO es "profesional". Para un formato profesional, necesitás controlar DÓNDE y CUÁNDO ocurren los saltos.

    ### Los tres tipos de salto

    | Salto | Atajo | ¿Qué hace? | ¿Cuándo usarlo? |
    |---|---|---|---|
    | **Salto de sistema** | `Enter` | Comienza un nuevo sistema en el compás seleccionado | Para controlar cuántos compases hay en cada sistema. Ej: "en este sistema quiero exactamente 4 compases, ni 3 ni 5". |
    | **Salto de página** | `Ctrl + Enter` | Comienza una nueva página en el compás seleccionado | Para controlar qué compases aparecen en cada página. Ej: "el clímax de la pieza (c. 45–52) debe estar completo en la página 3, sin cortes". |
    | **Salto de sección** | (paleta) | Nuevo sistema + reinicia numeración de compases, doble barra y armadura de cortesía | Para separar movimientos, secciones con cambio de tempo o carácter. |

    ### Dónde SÍ poner un salto de página

    - Después de una doble barra final de sección.
    - Después de un calderón que indica fin de frase importante.
    - Antes de un cambio de tempo o carácter (Allegro → Adagio).
    - Cuando el siguiente compás empieza una nueva idea musical claramente diferenciada.
    - Durante un silencio multicompás del instrumento (particellas).

    ### Dónde NO poner un salto de página

    - En medio de una ligadura de expresión (la ligadura se "rompe" visualmente).
    - En medio de un regulador (crescendo / diminuendo).
    - En medio de un tresillo o grupo irregular.
    - En medio de una frase musical (el músico "pierde el hilo" al pasar la página).
    - Durante un pasaje de alta densidad de notas (el músico no puede pasar la página mientras toca rápido).

    ### Cómo insertar y eliminar saltos

    **Insertar**:
    1. Seleccionar el compás donde querés el salto (clic en una nota o silencio de ese compás).
    2. Presionar `Enter` (salto de sistema), o `Ctrl + Enter` (salto de página), o arrastrar desde la paleta **Saltos y espaciadores**.

    **Eliminar**:
    1. Seleccionar el compás que tiene el salto.
    2. En la paleta **Propiedades de compás**, hacer clic en la "x" junto al tipo de salto.
    3. O seleccionar el salto directamente (clic en la línea punteada que aparece sobre el compás) y presionar `Suprimir`.

    !!! tip "Los saltos son binarios: o están o no están."
        Un error común: poner un salto de página "por las dudas" y luego olvidarse. Cuando corregís algo antes de ese compás, el salto de página se mantiene y puede quedar MAL puesto. Revisá TODOS los saltos antes de dar por terminada una partitura. Una partitura con saltos heredados de una revisión anterior es una partitura MAL formateada.

    ### El salto de sección: el más potente y el menos usado

    El salto de sección hace TRES cosas simultáneamente:
    1. Comienza un nuevo sistema (como el salto de sistema).
    2. Inserta una doble barra (separador visual de secciones).
    3. Opcionalmente: reinicia la numeración de compases, oculta/restaura la armadura de cortesía, y cambia el estilo de numeración.

    **Ejemplo**: tenés una sonata en tres movimientos (I. Allegro, II. Adagio, III. Presto) en UN SOLO archivo .mscz. Insertás un salto de sección al final del primer movimiento. El segundo movimiento empieza en página nueva, con doble barra, y con la numeración de compases reiniciada en 1. El músico lee "compás 1 del Adagio", no "compás 147 de la obra completa".

    > Insertar captura de una partitura con 3 saltos visibles: un salto de sistema (línea punteada sobre el compás), un salto de página (ícono de página), y un salto de sección (doble barra + línea punteada).

???+ note "Espaciadores: la herramienta de precisión"

    Los saltos de sistema y página controlan la ESTRUCTURA (dónde cortar). Los espaciadores controlan la AERACIÓN (cuánto espacio entre elementos).

    ### Tipos de espaciadores

    1. **Espaciador de pentagrama (Staff spacer)**:
        - Modifica la distancia entre un pentagrama y el siguiente DENTRO del mismo sistema.
        - Se inserta seleccionando un compás y arrastrando el ícono de "↓↑" desde la paleta **Saltos y espaciadores**.
        - Al arrastrar el punto azul hacia abajo, el pentagrama seleccionado se aleja del inferior. Hacia arriba, se acerca.
        - **Caso de uso**: en un sistema con 8 pentagramas, necesitás que los violines I estén más separados de los violines II para que las dinámicas del pentagrama superior no choquen con las notas del inferior.

    2. **Espaciador de sistema (System spacer)**:
        - Modifica la distancia entre DOS SISTEMAS consecutivos.
        - Útil cuando las indicaciones de tempo del sistema inferior (ej. "Allegro ♩ = 132") invaden el espacio del sistema superior.
        - También para cuando el último sistema de una página está muy pegado al borde inferior y necesita "aire".

    ### Reglas para espaciadores

    1. **Usalos con moderación.** Si necesitás espaciadores en CADA sistema, el problema no es de espaciadores: es de configuración global (Formato → Estilo → Página). Ajustá las distancias por defecto primero, y usá espaciadores solo para excepciones.
    2. **No abuses del espaciador hacia arriba.** Acercar demasiado dos pentagramas puede hacer que las notas de uno invadan el espacio del otro. Especialmente peligroso con pentagramas que tienen notas muy agudas (líneas adicionales superiores) y el pentagrama de arriba que tiene notas muy graves (líneas adicionales inferiores).
    3. **El espaciador de pentagrama se aplica al compás seleccionado y a todos los siguientes hasta el próximo espaciador.** Es "pegajoso". Si querés que el efecto se aplique a un solo sistema, insertá otro espaciador al inicio del siguiente sistema con el valor por defecto (0).

    > Insertar captura de la paleta "Saltos y espaciadores" con los distintos tipos de espaciadores visibles y un ejemplo de uso: un sistema con espaciador de pentagrama aplicado entre dos instrumentos.

---

## Actividad en Classroom

### Tarea: S26 — Formato de página y disposición

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S26_desorden.mscz`, una partitura de cuarteto de cuerdas (violín I, violín II, viola, violonchelo) de 48 compases con el formato de página deliberadamente caótico y múltiples errores de disposición; (b) `ejercicio_S26_formato.mscz`, una partitura para ensamble de cámara (flauta, clarinete en Si♭, piano) de 36 compases que requiere ser formateada desde cero para entrega profesional en A4 horizontal.

1. **Diagnóstico y corrección de formato.** Abrí `ejercicio_S26_desorden.mscz`:
    - Esta partitura de cuarteto de cuerdas está correctamente escrita en contenido musical, pero el formato es un DESASTRE. Diagnosticá al menos 8 problemas de formato:
        - Saltos de página mal puestos (cortan frases, dejan páginas casi vacías).
        - Compases con espaciado inconsistente (algunos muy anchos, otros aplastados).
        - Pentagramas demasiado juntos (dinámicas que chocan con otros pentagramas).
        - Sistemas mal distribuidos (último sistema de una página con un solo compás).
        - Márgenes inapropiados para el tamaño de papel.
        - Escala inadecuada (partitura microscópica o gigante).
        - Justificación inconsistente.
        - Falta de espaciadores donde son necesarios.
    - **Documentá** cada problema: compás afectado, qué está mal, por qué es un problema para el músico, y cómo lo corregiste.
    - Corregí TODOS los problemas. La partitura resultante debe verse PROFESIONAL y lista para imprimir.
    - Guardá como `APELLIDO_Nombre_S26_desorden_corregido.mscz`.

2. **Formateo desde cero para impresión profesional.** Abrí `ejercicio_S26_formato.mscz`:
    - Esta partitura para flauta, clarinete en Si♭ y piano está escrita pero SIN FORMATO (MuseScore aplicó su layout automático). Tu trabajo es formatearla para que sea una partitura de CÁMARA profesional lista para entregar a los músicos.
    - **Paso 1: Configuración de página**. Establecé:
        - Papel: A4 horizontal (297×210 mm).
        - Márgenes: superior 12 mm, inferior 15 mm, izquierdo 15 mm, derecho 12 mm.
        - Escala: ajustá el staff space hasta que la partitura se vea proporcionada (ni muy grande ni muy chica). Probá al menos 2 valores.
    - **Paso 2: Distribución de compases**. Decidí CUÁNTOS compases por sistema y CUÁNTOS sistemas por página. Insertá saltos de sistema y página donde corresponda. Criterios:
        - Ningún sistema debe tener menos de 2 ni más de 6 compases (dependiendo de la densidad rítmica).
        - Los saltos de página NO deben cortar frases musicales ni reguladores.
        - La última página NO debe tener un solo sistema (redistribuí para que quede al menos la mitad de la página ocupada).
    - **Paso 3: Espaciado**. Ajustá la distancia entre pentagramas y sistemas para que:
        - Los tres pentagramas de cada sistema estén claramente separados.
        - Las indicaciones de tempo y dinámicas no invadan pentagramas adyacentes.
        - El resultado sea "aireado" pero sin desperdiciar espacio.
    - **Paso 4: Ajustes finos**. Revisá estiramientos de compases individuales. Si hay compases con muchas semicorcheas junto a compases con redondas, ajustá para que el sistema se vea equilibrado.
    - Guardá como `APELLIDO_Nombre_S26_formato_profesional.mscz`.
    - Exportá como PDF: `APELLIDO_Nombre_S26_formato_profesional.pdf`.

3. **Comparación visual y funcional.** En Classroom, publicá una comparación de tu partitura formateada con la versión sin formato:
    - Captura de pantalla de UNA MISMA página en la versión sin formato (automática) y en tu versión corregida. Señalá al menos 5 diferencias en el formato con flechas o anotaciones.
    - Respondé: ¿qué mejora el formato profesional para el músico que va a leer la partitura? Mencioná al menos 3 beneficios concretos.

4. **Reflexión.** En Classroom, respondé:
    - ¿Cuál fue la decisión de formato más DIFÍCIL que tomaste en este ejercicio? ¿Por qué?
    - ¿Cuánto tiempo te llevó formatear correctamente la partitura? ¿Creés que es tiempo bien invertido o preferirías que MuseScore lo hiciera automáticamente siempre (aunque no quede perfecto)?
    - Si tuvieras que darle UN SOLO consejo de formato a un compañero que nunca formateó una partitura, ¿cuál sería?

### Entregables

- [ ] `APELLIDO_Nombre_S26_desorden_corregido.mscz`
- [ ] `APELLIDO_Nombre_S26_formato_profesional.mscz`
- [ ] `APELLIDO_Nombre_S26_formato_profesional.pdf`
- [ ] Comentario en Classroom con: (a) diagnóstico de 8+ problemas con su corrección, (b) comparación visual (imagen antes/después con anotaciones), (c) respuestas a las 4 preguntas de reflexión

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Diagnóstico | ≥8 problemas identificados, documentados y corregidos correctamente | 5–7 problemas corregidos | ≤4 problemas o documentación ausente |
| Configuración de página | Papel, márgenes y escala correctos; al menos 2 valores de staff space probados | Configuración básica correcta pero escala no probada | Sin configuración de página |
| Distribución de compases | Saltos de sistema y página puestos con criterio musical; última página balanceada; sin cortes en frases | Algunos saltos mal puestos o página final desbalanceada | Sin saltos manuales |
| Espaciado y ajustes | Distancias entre pentagramas y sistemas correctas; estiramientos individuales revisados; resultado profesional | Espaciado decente pero sin ajustes finos | Sin ajustes de espaciado |
| Comparación y reflexión | Comparación visual detallada con 3+ beneficios; respuestas con ejemplos concretos | Comparación presente pero superficial | Sin comparación ni reflexión |

---

*Basado en: MuseScore Studio 4 Handbook — Formatting: Page settings, Layout and formatting, Breaks and spacers | https://handbook.musescore.org*
