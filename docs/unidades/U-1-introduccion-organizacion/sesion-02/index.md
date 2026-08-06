# Sesión 2: Creación de una partitura nueva

📚 Handbook → Basics — Create new score, Instruments, Score properties | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="plantilla"></a> **Plantilla** | Archivo preconfigurado con instrumentos, estilos y diseño listos para empezar a escribir. MuseScore incluye plantillas para orquesta, banda, coro, piano y muchos más. |
    | <a id="instrumento"></a> **Instrumento** | Cada pentagrama individual o par de pentagramas dentro de una partitura. Puede ser un instrumento solista, una sección, o un sistema de varios pentagramas (como el piano). |
    | <a id="score"></a> **Score (partitura general)** | Documento principal que contiene todos los instrumentos de una obra. También se llama *partitura general* o *full score*. De él se extraen las particellas. |
    | <a id="armadura"></a> **Armadura de tonalidad** | Conjunto de sostenidos o bemoles al inicio del pentagrama que indica la tonalidad de la obra o sección. Afecta a las notas escritas, no a la reproducción en sí. |
    | <a id="compas"></a> **Indicación de compás** | Fracción numérica al inicio de la partitura (ej. 4/4, 3/4, 6/8) que define cuántos tiempos hay por compás y qué figura vale un tiempo. |
    | <a id="tempo"></a> **Tempo inicial** | Indicación de velocidad de la obra (ej. ♩ = 120). En MuseScore se configura durante la creación de la partitura y puede modificarse después con marcas de tempo. |
    | <a id="asistente"></a> **Asistente de nueva partitura** | Ventana paso a paso que guía la creación de un score nuevo: elige plantilla o instrumentos, configura armadura/compás/tempo y define datos de la partitura. |
    | <a id="transpositor"></a> **Instrumento transpositor** | Instrumento cuya nota escrita no coincide con la nota que suena (ej. clarinete en Si♭, trompa en Fa). MuseScore gestiona automáticamente la transposición si el instrumento se configura correctamente. |

???+ note "De la idea a la partitura: creación paso a paso"

    Toda partitura en MuseScore comienza con el **asistente de nueva partitura**. Accedés a él desde la pantalla de Inicio con el botón **Nueva partitura** o desde el menú **Archivo → Nuevo**.

    ![Asistente de nueva partitura en MuseScore](https://handbook.musescore.org/~gitbook/image?url=https%3A%2F%2F3455969201-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FP81HaeapLzzJGtG6DSwH%252Fuploads%252Fgit-blob-09de6ede505764b756e8ebffae21f656283e9741%252Fcreate-new-score-1440x900.gif%3Falt%3Dmedia&width=768&dpr=3&quality=100&sign=47ec765c&sv=2)

    El asistente tiene cuatro pasos:

    1. **Información general**: título, subtítulo, compositor, letrista, copyright.
    2. **Plantilla o instrumentos**: elegir una plantilla predefinida o construir el ensamble instrumento por instrumento.
    3. **Armadura de tonalidad**: seleccionar la tonalidad inicial.
    4. **Indicación de compás, tempo y número de compases**: establecer la métrica, la velocidad y la extensión.


    Una vez creada, la partitura se abre en la vista principal y todos estos parámetros pueden modificarse posteriormente desde el menú **Formato → Estilo → Partitura** o haciendo clic derecho sobre los elementos directamente en el score.

???+ note "Plantillas y selección de instrumentos"

    ### ¿Plantilla o desde cero?

    | Opción | Ventaja | Cuándo usarla |
    |---|---|---|
    | **Plantilla** | Instrumentos, orden, llaves y corchetes ya configurados. Lista para escribir. | Proyectos que siguen un formato estándar: orquesta, banda sinfónica, cuarteto de cuerdas, coro SATB, piano solo. |
    | **Desde cero** | Control total sobre qué instrumentos incluir, su orden y sus propiedades. | Ensambles no convencionales, combinaciones personalizadas, ejercicios con instrumentación específica. |


    ### Agregar, ordenar y eliminar instrumentos

    Si elegís "Elegir instrumentos" en lugar de una plantilla, el panel de selección de instrumentos permite:

    - **Buscar** un instrumento por nombre en el campo de búsqueda.
    - **Agregar** instrumentos al score con el botón `→` o doble clic.
    - **Reordenarlos** arrastrando el nombre en la lista de la derecha.
    - **Eliminarlos** con el botón `←` o la tecla Supr.

    !!! info "Orden convencional del score"
        El orden de los instrumentos en una partitura orquestal sigue una convención aceptada internacionalmente: maderas, metales, percusión, arpa/piano/celesta, cuerdas. Dentro de cada familia, del más agudo al más grave (flautín → flauta → oboe → corno inglés, etc.). Respetar este orden comunica profesionalismo y facilita la lectura del director.


???+ note "Datos de la partitura: título, compositor y más"

    Los metadatos de una partitura se ingresan en el primer paso del asistente, pero pueden editarse en cualquier momento desde **Archivo → Propiedades de la partitura** o **Propiedades del proyecto** (según la versión).

    Campos principales:

    | Campo | Visible en | Ejemplo |
    |---|---|---|
    | **Título** | Primera página del score y de cada particella | *Cuarteto de cuerdas No. 1* |
    | **Subtítulo** | Debajo del título | *Movimiento I — Allegro* |
    | **Compositor** | Margen derecho, primera página | *José Urgilés* |
    | **Letrista** | Margen izquierdo, primera página | *Texto de María García* |
    | **Copyright** | Pie de la primera página | *© 2026* |

    Estos datos se insertan automáticamente en marcos de texto sobre la primera página. Si no los completás durante la creación, la partitura aparecerá sin título visible hasta que los agregues manualmente.

???+ note "Armadura, compás y tempo inicial"

    Los pasos 3 y 4 del asistente configuran tres elementos fundamentales que pueden cambiarse en cualquier momento de la edición:

    ### Armadura de tonalidad

    La armadura se selecciona de una lista que recorre todas las tonalidades mayores y menores. MuseScore muestra la cantidad de sostenidos o bemoles correspondientes.

    - Si la obra **no tiene una tonalidad definida**, elegí "Do mayor / La menor" (sin alteraciones) o usá una armadura abierta/atonal desde la paleta.
    - Si la obra **cambia de tonalidad** más adelante, no te preocupes: podés insertar cambios de armadura en cualquier compás.

    ### Indicación de compás

    Elegí entre los compases más comunes (4/4, 3/4, 2/4, 6/8, etc.) o escribí un compás personalizado. MuseScore ajusta automáticamente la barra de compás y la agrupación de figuras según la métrica elegida.

    ### Tempo inicial

    Se expresa como una figura musical igual a un número de pulsos por minuto (BPM). Por ejemplo:
    - ♩ = 120 (negra a 120 BPM, moderado)
    - ♩ = 60 (lento)
    - ♩ = 180 (rápido)

    También podés escribir texto de tempo (ej. "Allegro", "Andante") y MuseScore ajustará la reproducción en consecuencia. El texto de tempo es **independiente** del valor BPM: podés mostrar "Allegro" y configurar internamente ♩ = 132.


---

## Actividad en Classroom

### Tarea: S02 — Plantilla de ensamble correctamente preparada

1. **Creá dos partituras desde cero** usando el asistente de nueva partitura:
   - **Partitura A: Cuarteto de cuerdas** (violín I, violín II, viola, violoncello). Usá la plantilla "Cuarteto de cuerdas". Tonalidad: Re mayor. Compás: 4/4. Tempo: ♩ = 100. 32 compases.
   - **Partitura B: Pequeño ensamble de vientos** (flauta, oboe, clarinete en Si♭, fagot). Elegí los instrumentos manualmente. Tonalidad: Fa mayor. Compás: 3/4. Tempo: ♩ = 80. 24 compases.

2. **Completá los metadatos** de ambas partituras: título, compositor (tu nombre), y subtítulo con el tipo de ensamble.

3. **Verificá** que el orden de los instrumentos sigue la convención de agudos a graves dentro de cada familia.

4. **Revisá** los nombres completos y abreviados de cada instrumento. En la Partitura B, asegurate de que el clarinete aparece como "Clarinete en Si♭" y no solo "Clarinete".

5. **Exportá ambas partituras a PDF** y guardá los archivos .mscz correspondientes.

### Entregables

- [ ] `APELLIDO_Nombre_S02_CuartetoCuerdas_v01.mscz`
- [ ] `APELLIDO_Nombre_S02_CuartetoCuerdas_v01.pdf`
- [ ] `APELLIDO_Nombre_S02_EnsambleVientos_v01.mscz`
- [ ] `APELLIDO_Nombre_S02_EnsambleVientos_v01.pdf`

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Instrumentación correcta | Ambas partituras tienen los instrumentos solicitados en el orden convencional | Una partitura tiene error de orden u omisión | Faltan instrumentos en ambas |
| Metadatos completos | Título, compositor y subtítulo presentes en ambas | Falta un metadato en una partitura | Sin metadatos |
| Armadura, compás, tempo | Las tres configuraciones coinciden con lo solicitado en ambas | Un error en una partitura | Varios errores o configuraciones omitidas |
| Exportación y nombres | 4 archivos entregados con la convención de nombres correcta | Falta un archivo o el nombre no sigue la convención | No se entregaron los archivos |

---

*Basado en: MuseScore 3 Handbook — Basics: Create new score, Instruments, Score properties | https://musescore.org/en/handbook/3*
