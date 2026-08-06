# Sesión 24: Importación y exportación MusicXML

📚 Handbook → Advanced topics: File formats (MusicXML), Save/Export/Print | Herramientas: MuseScore Studio 4, Google Classroom, archivos MusicXML de otros editores

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="musicxml"></a> **MusicXML** | Formato abierto de intercambio de partituras digitales basado en XML. A diferencia de MIDI (que transmite instrucciones de ejecución), MusicXML transmite SEMÁNTICA MUSICAL: nombres de notas, duraciones, armaduras, matices, texto, letra, articulaciones, y la ESTRUCTURA de la partitura (compases, sistemas, páginas). Es el formato universal para mover partituras entre diferentes programas de notación. |
    | <a id="xml"></a> **XML (eXtensible Markup Language)** | Lenguaje de marcado que estructura información en etiquetas anidadas: `<note><pitch><step>C</step><octave>4</octave></pitch><duration>256</duration></note>`. MusicXML está construido sobre XML. Un archivo .musicxml o .mxl se puede abrir con un editor de texto y ES LEGIBLE (a diferencia de un archivo binario como .mscz o .musx). |
    | <a id="mxl"></a> **.MXL (MusicXML comprimido)** | Versión comprimida (ZIP) del archivo MusicXML. Un archivo .mxl es típicamente 20 veces más pequeño que su equivalente .musicxml sin comprimir. MuseScore abre y guarda ambos formatos. Para enviar por correo o publicar en internet, usar .mxl. Para edición manual del XML o procesos automatizados, usar .musicxml sin comprimir. |
    | <a id="intercambio"></a> **Intercambio entre editores (cross-application workflow)** | Flujo de trabajo donde una partitura creada en el programa A (ej. Finale, Sibelius, Dorico) se exporta como MusicXML, se abre en el programa B (MuseScore), se edita, y potencialmente se reexporta de vuelta al programa A. MusicXML es el "idioma común" que permite esta interoperabilidad. |
    | <a id="roundtrip"></a> **Roundtrip (viaje de ida y vuelta)** | Proceso de exportar una partitura de MuseScore a MusicXML y luego reimportar ese mismo MusicXML de vuelta a MuseScore. Idealmente debería ser "sin pérdida" (la partitura se ve igual). En la práctica, ciertos elementos pueden perderse o modificarse: fuentes personalizadas, ciertos tipos de líneas, configuraciones avanzadas de formato. |
    | <a id="musicxml-perdida"></a> **Pérdida en la conversión (conversion loss)** | Elementos de la partitura que NO sobreviven al proceso de exportación + importación vía MusicXML. Cada programa implementa el estándar MusicXML con diferentes grados de completitud. Lo que MuseScore exporta puede no ser interpretado correctamente por Finale, y viceversa. Los elementos más problemáticos suelen ser: formato de página, espaciado de pentagramas, fuentes no estándar, y ciertos tipos de líneas. |
    | <a id="doctype-musicxml"></a> **DOCTYPE y versión de MusicXML** | MusicXML tiene versiones (1.0, 2.0, 3.0, 3.1, 4.0). MuseScore 4 exporta MusicXML 4.0 por defecto, pero puede exportar versiones anteriores para compatibilidad con programas más antiguos. La versión se especifica en el DOCTYPE al inicio del archivo XML: `<!DOCTYPE score-partwise PUBLIC "-//Recordare//DTD MusicXML 4.0 Partwise//EN">`. |
    | <a id="partwise"></a> **Partwise vs. Timewise** | Dos "sabores" de MusicXML: Partwise organiza la partitura por PARTE (primero toda la flauta, luego todo el violín). Timewise organiza por COMPÁS (compás 1 de todos los instrumentos, compás 2 de todos los instrumentos). MuseScore usa Partwise (el más común). La mayoría de los editores soportan ambos pero prefieren Partwise. |
    | <a id="semantica-vs-presentacion"></a> **Semántica vs. Presentación** | MusicXML prioriza la SEMÁNTICA (qué significan los símbolos) sobre la PRESENTACIÓN (cómo se ven en la página). Esto es bueno para el intercambio entre programas (cada programa decide cómo dibujar una dinámica *ff*) pero malo para preservar el formato exacto de página (los saltos de línea y página raramente se preservan). |
    | <a id="musicxml-vs-midi"></a> **MusicXML vs. MIDI para intercambio** | MusicXML preserva la notación (armaduras, matices, texto, articulaciones). MIDI preserva la interpretación (velocity, tempo, controladores). Si querés mover una partitura entre editores → MusicXML. Si querés mover una interpretación entre secuenciadores → MIDI. Son complementarios, no competidores. |
    | <a id="pdf-export"></a> **Exportación a PDF** | Proceso de convertir la partitura de MuseScore en un archivo PDF (Portable Document Format) que mantiene el formato visual exacto independientemente de la computadora donde se abra. El PDF es el formato de ENTREGA final: el director de orquesta, los músicos y la imprenta reciben PDFs, no archivos .mscz. |
    | <a id="mscz"></a> **.MSCZ (formato nativo de MuseScore)** | Formato propietario de MuseScore (comprimido). Contiene TODA la información de la partitura: notas, formato, estilos, paletas personalizadas, configuraciones de reproducción. Es el formato que debés usar para GUARDAR tu trabajo. MusicXML y MIDI son para INTERCAMBIAR. MSCZ es para TRABAJAR. |

???+ note "MusicXML: el esperanto de las partituras digitales"

    Si MIDI es el idioma de la interpretación, MusicXML es el idioma de la NOTACIÓN. Entender cuándo usar cada uno es una habilidad profesional fundamental.

    ### ¿Por qué existe MusicXML?

    Imaginá que escribiste una sinfonía completa en Finale durante 3 meses. Ahora querés pasarte a MuseScore (o a Dorico, o a Sibelius). Sin MusicXML, tus opciones son:
    1. Reescribir TODO desde cero (semanas de trabajo).
    2. Exportar como MIDI a MuseScore y... obtener un desastre que requiere días de limpieza (como viste en la Sesión 23).
    3. Exportar como PDF y... tener una imagen, no una partitura editable.

    MusicXML resuelve este problema. Es un formato ABIERTO (no pertenece a ninguna empresa) diseñado específicamente para intercambiar partituras entre programas de notación preservando la máxima cantidad de información musical posible.

    ### La diferencia fundamental

    | Característica | MIDI | MusicXML |
    |---|---|---|
    | ¿Qué representa? | Eventos de ejecución (nota ON, nota OFF, velocity, pedal) | Símbolos de notación (negra, clave de Sol, *mf*, ligadura) |
    | ¿Las notas tienen nombre? | No. Solo "nota número 60" (= Do₄). No sabe si es Do♯ o Re♭. | Sí. `<step>D</step><alter>-1</alter><octave>4</octave>` (= Re♭₄). |
    | ¿Preserva el compás? | Parcialmente (mensajes de time signature) | Sí. `<time><beats>4</beats><beat-type>4</beat-type></time>` |
    | ¿Preserva la armadura? | Parcialmente | Sí, con alteraciones precisas |
    | ¿Preserva articulaciones? | No (solo afecta velocity y duración) | Sí (staccato, acento, fermata, etc.) |
    | ¿Preserva dinámicas? | Parcialmente (CC7 = volumen, no *p* o *f*) | Sí (*p*, *mf*, *f*, *cresc.*, etc.) |
    | ¿Preserva texto y letra? | Solo en .KAR y limitado | Sí (título, compositor, letra, indicaciones de tempo, texto de ensayo) |
    | ¿Preserva el formato de página? | No | Parcialmente (márgenes, tamaño de página, pero no saltos exactos) |
    | ¿Es legible por humanos? | No (binario) | Sí (texto XML, aunque complejo) |

    !!! tip "La regla de intercambio"
        **Para mover entre editores de partituras → MusicXML. Para mover entre secuenciadores o DAWs → MIDI. Para escuchar → exportá audio (MP3/WAV).**

    ### Historia breve: de los formatos propietarios al estándar abierto

    - **1990s**: cada editor de partituras tenía su propio formato cerrado. Finale usaba .mus, Sibelius usaba .sib, capella usaba .cap. Las partituras estaban ENCERRADAS en el programa que las creó.
    - **2000**: Michael Good (fundador de Recordare) crea MusicXML 1.0 basado en su trabajo de doctorado. La idea era simple: un formato basado en XML (como HTML pero para música) que cualquier programa pudiera leer y escribir.
    - **2004–2011**: adopción gradual. Finale fue el primer gran editor en soportar MusicXML. Sibelius siguió después. Para 2011, prácticamente todos los editores de partituras lo soportaban.
    - **2015**: MusicXML se convierte en un estándar abierto mantenido por el W3C (el mismo consorcio que mantiene HTML).
    - **2021**: MusicXML 4.0. MuseScore 4 lo soporta nativamente.

    Hoy, MusicXML es el formato estándar de facto para intercambio de partituras. Si un programa de notación NO soporta MusicXML, está desconectado del ecosistema.

???+ note "Exportar desde MuseScore a MusicXML"

    Exportar una partitura de MuseScore a MusicXML es la operación MÁS COMÚN cuando necesitás compartir tu trabajo con alguien que usa otro editor.

    ### Procedimiento

    1. **Archivo → Exportar** (o `Ctrl / Cmd + E`).
    2. En el diálogo de exportación, en el desplegable **Formato**, seleccionar:
       - **MusicXML sin comprimir (.musicxml)**: archivo de texto XML, legible, más grande. Útil para procesamiento automatizado o inspección manual.
       - **MusicXML comprimido (.mxl)**: archivo ZIP, más chico (~20× menor). Recomendado para intercambio general.
    3. Elegir ubicación y nombre de archivo.
    4. Clic en **Guardar**.

    ### Opciones de exportación

    | Opción | Descripción | Recomendación |
    |---|---|---|
    | **Versión de MusicXML** | 4.0 (más moderna), 3.1, 3.0, 2.0 (más compatible) | Usar 4.0 a menos que el programa destino requiera una versión anterior |
    | **Exportar solo selección** | Exporta únicamente los compases/notas seleccionados | Útil para compartir fragmentos, no partituras completas |
    | **Incluir información de formato de página** | Agrega dimensiones de página (tamaño A4, márgenes) al MusicXML | Activado: ayuda a mantener el formato. Pero si el programa destino ignora esta información, no hay garantía. |

    ### Qué se exporta BIEN (≈ 95% de fidelidad)

    - Notas, duraciones, alturas, alteraciones
    - Armaduras, compases, claves
    - Matices (dinámicas, reguladores)
    - Articulaciones (staccato, acento, tenuto, fermata)
    - Ligaduras de expresión y de prolongación
    - Texto (título, compositor, indicaciones de tempo, letra, texto de pentagrama)
    - Cifrado armónico
    - Saltos de línea y de página
    - Márgenes y tamaño de página

    ### Qué se exporta REGULAR (≈ 70–80% de fidelidad)

    - Líneas (octava, pedal, trinos): se exportan pero pueden perder formato exacto
    - Voces múltiples: se exportan pero la asignación de plicas puede cambiar
    - Tresillos y valores irregulares: se exportan bien en versiones 3.1+

    ### Qué NO se exporta bien (< 50% de fidelidad)

    - Fuentes personalizadas de texto
    - Imágenes incrustadas en la partitura
    - Configuraciones avanzadas de espaciado manual
    - Ciertos tipos de líneas personalizadas creadas con la paleta "Líneas"
    - Configuraciones del mezclador de audio (efectos, balance)
    - Paletas personalizadas


???+ note "Importar MusicXML en MuseScore"

    ### Desde otro editor de partituras

    Si recibiste un archivo .musicxml o .mxl desde Finale, Sibelius, Dorico o cualquier otro editor:

    1. **Archivo → Abrir** (o arrastrar el archivo a la ventana de MuseScore).
    2. MuseScore detecta que es MusicXML y lo abre directamente.
    3. La partitura aparece inmediatamente. NO hay diálogo de importación como con MIDI.

    ### Qué verificar después de importar

    La importación de MusicXML es mucho más limpia que la de MIDI, pero siempre verificá:

    1. **Armadura y compás**: al inicio de la partitura. Generalmente correctos.
    2. **Alteraciones accidentales**: verificá que no haya enarmonías extrañas.
    3. **Ligaduras**: las de expresión y prolongación pueden "romperse" al cruzar saltos de línea.
    4. **Texto**: verificá que tildes y caracteres especiales (ñ, ü, ç) se hayan preservado.
    5. **Formato de página**: es LO PRIMERO que se pierde. Esperá tener que reajustar saltos de línea y sistema.
    6. **Fuentes**: si el programa original usaba fuentes no estándar, MuseScore las sustituye por sus fuentes por defecto. El texto se preserva pero la apariencia cambia.

    !!! warning "El formateo de página NO se preserva bien"
        Este es el principal punto de dolor. Una partitura de Finale perfectamente formateada, al importarla en MuseScore vía MusicXML, casi siempre requiere reajuste de saltos de sistema, espaciado de pentagramas y distribución de compases. Esto NO es un error de MuseScore: es una limitación del estándar MusicXML, que prioriza el contenido musical sobre la presentación visual.

    ### Desde una versión antigua de MuseScore

    Si estás migrando de MuseScore 3 a MuseScore 4, NO uses MusicXML. MuseScore 4 abre archivos .mscz de MuseScore 3 directamente (y los convierte automáticamente). Usá MusicXML solo para intercambio entre programas de diferentes fabricantes.


???+ note "Exportación de audio y PDF: los formatos de entrega"

    MusicXML y MIDI son formatos de INTERCAMBIO entre programas. Pero cuando la partitura está terminada, necesitás formatos de ENTREGA para compartir con personas que no usan MuseScore.

    ### PDF: el estándar universal de partituras

    El PDF es el formato que reciben los músicos, directores, editoriales e imprentas.

    **Exportar PDF desde MuseScore**:
    1. **Archivo → Exportar**.
    2. Seleccionar formato **PDF**.
    3. **IMPORTANTE**: activar la opción **"Exportar partes individuales"** si la partitura tiene particellas (partes extraídas para cada instrumento). Esto genera un PDF por cada instrumento, más el de la partitura completa.
    4. Guardar.

    **Verificación pre-PDF** (checklist antes de exportar):
    - [ ] ¿Los títulos, compositor y metadatos están completos y correctos?
    - [ ] ¿Los saltos de página son los correctos (no hay páginas a medio llenar ni pasajes cortados)?
    - [ ] ¿La letra (si hay) está sincronizada y sin errores ortográficos?
    - [ ] ¿Las dinámicas y articulaciones son legibles y no se solapan?
    - [ ] ¿Los números de compás son correctos y visibles?
    - [ ] ¿Hay una página de portada o al menos título y compositor en la primera página?
    - [ ] ¿Las partes individuales tienen el nombre del instrumento y los mismos números de compás que la partitura completa?

    ### Audio: para escuchar sin MuseScore

    | Formato | Ventaja | Desventaja | Cuándo usarlo |
    |---|---|---|---|
    | **MP3** | Tamaño pequeño, compatible con todo | Calidad con pérdida (comprimido) | Compartir por internet, enviar por correo, subir a Classroom |
    | **WAV** | Calidad sin pérdida (CD quality) | Archivos grandes (10 MB/minuto) | Archivado maestro, uso profesional, mezcla posterior en DAW |
    | **OGG / FLAC** | Códec libre, buena compresión | Menos compatible que MP3 | Uso en proyectos de código abierto |

    **Procedimiento**:
    1. **Archivo → Exportar**.
    2. Formato: **MP3** o **WAV**.
    3. MuseScore renderiza (genera) el audio usando los sonidos configurados en el sintetizador.
    4. La velocidad depende de la complejidad y duración de la partitura.

    !!! tip "El audio de MuseScore es una guía, no un producto final"
        Los sonidos por defecto de MuseScore (soundfont MS Basic) son funcionales pero NO son de calidad profesional. Si necesitás audio de alta calidad para una producción, exportá el MIDI y abrirlo en un DAW (Reaper, Logic, Ableton) con librerías de sonido profesionales (orquesta virtual, piano sampleado). El audio de MuseScore sirve para "darte una idea de cómo suena", no para un álbum.

---

## Actividad en Classroom

### Tarea: S24 — Importación y exportación MusicXML

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S24_finale.musicxml`, una partitura de cuarteto de cuerdas (violín I, violín II, viola, violonchelo) de 24 compases en Re mayor, exportada desde Finale, Finale Notepad o cualquier editor que genere MusicXML con sus propias convenciones de formato; (b) `ejercicio_S24_desordenado.mscz`, una partitura de MuseScore ya escrita pero con errores deliberados de formato y contenido que debe ser verificada, corregida y exportada en todos los formatos; (c) `ejercicio_S24_partitura.mscz`, una partitura completa para piano solo en Mi menor, 32 compases, lista para generar particellas.

1. **Importación desde otro editor.** Abrí `ejercicio_S24_finale.musicxml` en MuseScore:
    - La partitura fue creada en Finale (o Sibelius, Dorico, etc.) y exportada como MusicXML. Al abrirla en MuseScore, notá las diferencias.
    - **Diagnóstico**: documentá al menos 5 diferencias entre cómo se veía en el editor original (o cómo debería verse) y cómo se ve en MuseScore. Prestá atención a: formato de página, fuentes del texto, posición de matices, saltos de sistema, dirección de plicas, aspecto de las ligaduras.
    - **Corrección**: ajustá el formato para que la partitura sea correcta y profesional en MuseScore. Reacomodá saltos de página, verificá el texto (título, compositor), ajustá la posición de dinámicas si están mal ubicadas.
    - **Verificación**: ¿la música suena igual en MuseScore que en el editor original? Reproducí y compará. Anotá cualquier diferencia auditiva.
    - Guardá como `APELLIDO_Nombre_S24_importado.mscz`.

2. **Exportación a todos los formatos.** Abrí `ejercicio_S24_desordenado.mscz`:
    - Esta partitura fue preparada con errores deliberados. Encontrá y corregí:
        - Al menos 2 errores de formato de página (saltos de página incorrectos, compases que quedan solos en un sistema).
        - Al menos 2 errores de texto (faltan metadatos, título incompleto, compositor ausente).
        - Al menos 2 elementos de notación que se verían mal al exportar (dinámicas superpuestas, ligaduras rotas en saltos de línea).
        - Verificá que las alteraciones y enarmonías sean correctas.
    - Una vez corregida, exportá la partitura en TODOS estos formatos:
        - `APELLIDO_Nombre_S24_desordenado.mscz` (formato nativo de MuseScore, corregido)
        - `APELLIDO_Nombre_S24_desordenado.musicxml` (MusicXML sin comprimir)
        - `APELLIDO_Nombre_S24_desordenado.mxl` (MusicXML comprimido)
        - `APELLIDO_Nombre_S24_desordenado.mid` (MIDI)
        - `APELLIDO_Nombre_S24_desordenado.pdf` (PDF)
        - `APELLIDO_Nombre_S24_desordenado.mp3` (audio MP3)
    - **Prueba de roundtrip**: abrí el archivo `APELLIDO_Nombre_S24_desordenado.musicxml` que ACABÁS de exportar. Comparalo con el .mscz original corregido. ¿Qué diferencias encontrás? ¿Se perdió algo en el viaje de ida y vuelta? Documentá.

3. **Generación de particellas.** Abrí `ejercicio_S24_partitura.mscz`:
    - Esta partitura de piano solo NO tiene particellas porque el piano es un solo instrumento, PERO contiene pasajes que serían buenos candidatos para particellas si fuera una partitura de ensamble. Para este ejercicio, imaginá que es una partitura para Piano + Flauta (la mano derecha del piano es la melodía de la flauta).
    - **Separar las voces**: extraé la melodía (mano derecha, pentagrama superior) a un pentagrama independiente para Flauta. Conservá el acompañamiento (mano izquierda) en el pentagrama de piano.
    - **Crear particellas**: con la nueva partitura para Flauta + Piano, generá las particellas: **Archivo → Partes → Generar todas las partes**.
    - **Formatear las particellas**: abrí cada parte individualmente y verificá:
        - Nombre del instrumento visible.
        - Números de compás correctos y sincronizados con la partitura completa.
        - Saltos de página lógicos (no cortar frases musicales).
        - Silencios de espera (si el instrumento NO toca durante varios compases, deben aparecer los silencios multicompás).
    - Exportá cada parte como PDF individual y la partitura completa como PDF.
    - Exportá la partitura completa como MusicXML.

4. **Integración: flujo de trabajo inter-editor.** Buscá en internet o usá un editor de partituras alternativo (Finale Notepad es gratuito, Sibelius First es gratuito, Flat.io es online, Noteflight es online) para:
    - Crear una partitura NUEVA de al menos 12 compases en el editor externo (NO MuseScore). Debe tener al menos: una melodía, cifrado armónico, 2 indicaciones de dinámica, 1 articulación, título y compositor.
    - Exportarla como MusicXML desde ese editor.
    - Importarla en MuseScore.
    - Documentá el proceso: ¿qué editor usaste? ¿qué se preservó bien? ¿qué se perdió o cambió?
    - Completá la siguiente tabla comparativa en Classroom:

    | Elemento | ¿Se preservó correctamente? (Sí/No/Parcial) | Observaciones |
    |---|---|---|
    | Notas y duraciones | | |
    | Armadura y compás | | |
    | Dinámicas | | |
    | Articulaciones | | |
    | Cifrado armónico | | |
    | Texto (título, compositor) | | |
    | Formato de página | | |
    | Fuentes de texto | | |

    - Guardá el MusicXML original, el .mscz importado y el PDF de ambos.

5. **Reflexión sobre formatos de intercambio.** En Classroom, respondé:
    - Si un colega te pide "pasame la partitura para editarla en mi programa", ¿qué formato le enviarías: MIDI o MusicXML? ¿Por qué? ¿Qué información perdería si le mandás el formato incorrecto?
    - Después del roundtrip (exportar como MusicXML y reimportar), ¿qué elementos se perdieron o modificaron? ¿Esto te parece aceptable o es un defecto grave? Justificá.
    - ¿Por qué existen TANTOS formatos (.mscz, .musicxml, .mxl, .mid, .mp3, .pdf)? ¿No sería más fácil tener UN SOLO formato que lo haga todo? Explicá por qué cada formato tiene un propósito diferente.

### Entregables

- [ ] `APELLIDO_Nombre_S24_importado.mscz` (MusicXML importado desde otro editor y corregido)
- [ ] `APELLIDO_Nombre_S24_importado.pdf`
- [ ] `APELLIDO_Nombre_S24_desordenado.mscz` (corregido)
- [ ] `APELLIDO_Nombre_S24_desordenado.musicxml`
- [ ] `APELLIDO_Nombre_S24_desordenado.mxl`
- [ ] `APELLIDO_Nombre_S24_desordenado.mid`
- [ ] `APELLIDO_Nombre_S24_desordenado.pdf`
- [ ] `APELLIDO_Nombre_S24_desordenado.mp3`
- [ ] `APELLIDO_Nombre_S24_partitura_completa.pdf` (partitura completa de piano + flauta)
- [ ] `APELLIDO_Nombre_S24_flauta.pdf` (particella de flauta)
- [ ] `APELLIDO_Nombre_S24_piano.pdf` (particella de piano)
- [ ] `APELLIDO_Nombre_S24_partitura_completa.musicxml`
- [ ] `APELLIDO_Nombre_S24_intereditor.mscz` (importado del editor externo)
- [ ] `APELLIDO_Nombre_S24_intereditor_original.musicxml` (archivo original del editor externo)
- [ ] `APELLIDO_Nombre_S24_intereditor.pdf`
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) tabla comparativa de preservación de elementos (Parte 4), (c) diferencias encontradas en el roundtrip (Parte 2), (d) nombre del editor externo usado (Parte 4)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Importación desde otro editor | ≥5 diferencias identificadas y corregidas; formato ajustado; partitura profesional en MuseScore | 3–4 diferencias corregidas | ≤2 diferencias o sin corrección |
| Exportación multiformato | 6 formatos exportados correctamente; partitura corregida antes de exportar; roundtrip documentado | 4–5 formatos o roundtrip sin documentar | ≤3 formatos |
| Particellas | Partes generadas y formateadas; nombres, números de compás, saltos de página correctos; PDFs exportados | Partes generadas pero con errores de formato | Sin particellas |
| Flujo inter-editor | Partitura creada en editor externo y MusicXML importado en MuseScore; tabla comparativa completa; diferencias documentadas | Proceso completado pero tabla incompleta | Sin flujo inter-editor |
| Reflexión | 3 respuestas con análisis de formatos, pérdida de información y propósito de cada formato | 2 respuestas correctas | ≤1 respuesta o superficial |

---

*Basado en: MuseScore Studio 4 Handbook — File formats (MusicXML), Save/Export/Print | https://handbook.musescore.org*
