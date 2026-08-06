# Sesión 29: Exportación y formatos de entrega

📚 Handbook → Basics: Open/Save/Export/Print | Advanced topics: File formats | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="mscz"></a> **.mscz** | Formato nativo comprimido de MuseScore. Contiene TODO (notas, formato, sonidos, imágenes). ES tu archivo de trabajo. Solo lo abre MuseScore. |
    | <a id="mscx"></a> **.mscx** | Formato nativo SIN comprimir de MuseScore. Es XML legible. Útil para control de versiones con Git, porque permite ver diferencias entre versiones. Ocupa más espacio. |
    | <a id="mxl"></a> **.mxl / MusicXML comprimido** | Formato de intercambio ENTRE editores de partituras. Comprimido (ZIP). Lo abren MuseScore, Finale, Sibelius, Dorico y otros. Preserva contenido musical pero PIERDE formato de página y fuentes. |
    | <a id="musicxml"></a> **.musicxml (sin comprimir)** | Igual que .mxl pero SIN comprimir (XML plano). Archivos ENORMES. Útil para procesamiento automático o inspección, pero NO para compartir. |
    | <a id="mid-format"></a> **.mid (MIDI)** | Formato de secuenciación. Contiene números de nota, velocity, tempo, programa. NO contiene notación visual. Se usa para llevar música a DAWs (Ableton, Logic, Reaper). |
    | <a id="pdf"></a> **.pdf (Portable Document Format)** | Formato de documento vectorial. Se ve EXACTAMENTE igual en cualquier computadora. Estándar para impresión y publicación de partituras. NO es editable sin software especializado. |
    | <a id="png-svg"></a> **.png vs .svg** | PNG: imagen raster (pixeles). Se pixela al ampliar. Para web o redes sociales. SVG: imagen vectorial (fórmulas matemáticas). Escalable a cualquier tamaño sin pérdida. Para diseño gráfico. |
    | <a id="mp3-wav-flac"></a> **.mp3 / .wav / .flac** | Formatos de audio. MP3: comprimido con pérdida (chico, para compartir). WAV: sin comprimir (ENORME, calidad máxima). FLAC: comprimido sin pérdida (mitad del tamaño de WAV, misma calidad). |
    | <a id="bitrate"></a> **Bitrate (tasa de bits)** | Cantidad de datos por segundo en un archivo de audio comprimido. Más bitrate = mejor calidad = archivo más grande. MP3 estándar: 128–320 kbps. |
    | <a id="sample-rate"></a> **Sample rate (frecuencia de muestreo)** | Cuántas "fotos" del sonido por segundo toma el archivo de audio. Estándar CD: 44100 Hz. Mayor sample rate = mayor fidelidad... hasta cierto punto. |
    | <a id="normalizar"></a> **Normalizar (normalize)** | Ajustar el volumen global del audio para que el punto más fuerte NO distorsione (clipping) y el más suave sea audible. Activar SIEMPRE al exportar audio. |
    | <a id="batch-export"></a> **Exportación masiva (batch export)** | Exportar TODAS las partes de una partitura en UNA sola operación. Ejemplo: exportar 12 partes como PDF en un solo paso en lugar de 12 exportaciones individuales. |
    | <a id="roundtrip"></a> **Roundtrip** | Ciclo completo de exportar una partitura a otro formato y luego REIMPORTARLA. Sirve para medir CUÁNTA información se pierde en el proceso. Ejemplo: .mscz → .mxl → reimportar .mxl en MuseScore. |
    | <a id="metadatos"></a> **Metadatos (metadata)** | Información INVISIBLE dentro del archivo: título, compositor, copyright, fecha. Viaja con el archivo. Un PDF sin metadatos aparece como "Untitled" en cualquier visor. |

???+ note "El ecosistema de formatos: cada archivo cuenta una historia diferente"

    Terminaste tu obra. La escribiste en MuseScore. Generaste las partes. Todo está perfecto. Ahora... ¿qué archivo entregás a quién?

    Tres personas te piden tu música:

    | Persona | Necesita | ¿Qué le mandás? |
    |---|---|---|
    | Tu profesor de composición | EDITAR tu partitura en su programa | MusicXML (.mxl) |
    | El director del ensamble | IMPRIMIR las partes para el ensayo | PDF |
    | Tu amigo productor | ESCUCHAR cómo suena para ponerla en un demo | MP3 o WAV |

    **El mismo contenido musical. Tres formatos distintos. Tres propósitos diferentes.**

    ### La tabla maestra de formatos

    | Formato | Tipo | ¿Para quién? | ¿Qué preserva? | ¿Qué PIERDE? |
    |---|---|---|---|---|
    | **.mscz** | Nativo comprimido | Para VOS | TODO (notas, formato, sonidos) | NADA |
    | **.mxl** | Intercambio comprimido | Otro editor de partituras | Notas, ritmos, texto, dinámicas | Formato de página, fuentes, espaciado |
    | **.mid** | Secuenciación | DAW (Ableton, Logic, Reaper) | Notas, tempo, velocidad | TODO lo visual, matices como velocity |
    | **.pdf** | Documento vectorial | Imprenta, atril | Apariencia visual EXACTA | No editable |
    | **.png** | Imagen raster | Web, redes sociales | Lo que se ve en pantalla | No editable, se pixela al ampliar |
    | **.svg** | Imagen vectorial | Diseño gráfico, Illustrator | Gráfico escalable | No es partitura editable |
    | **.mp3** | Audio comprimido | Distribución general | Sonido aceptable, archivo chico | Calidad (compresión con pérdida) |
    | **.wav** | Audio sin comprimir | Estudio, mezcla, masterización | Sonido en máxima calidad | Archivo ENORME |
    | **.flac** | Audio comprimido sin pérdida | Archivo alta calidad | Sonido perfecto, mitad del WAV | Compatibilidad limitada |

    !!! tip "Regla mnemotécnica"
        **mscz** → Mi Seguro (de) Conservarlo (en) Zip. Guardalo SIEMPRE. Es tu backup perfecto.  
        **mxl** → Mi XML Ligero. Para compartir CON otros editores.  
        **mid** → Música (sin) Imagen Digital. Para máquinas.  
        **pdf** → Para Distribución Final. Para humanos que LEEN.  
        **mp3** → Música Para 3 segundos (de descarga). Para humanos que ESCUCHAN.

???+ note "Exportación de audio: no es solo 'Archivo → MP3'"

    Cuando exportás audio desde MuseScore, hay decisiones técnicas que afectan la calidad del resultado.

    ### El diálogo de exportación de audio

    **Archivo → Exportar → Exportar...** y seleccionar formato de audio (MP3, WAV, FLAC, OGG).

    #### 1. Elegir el formato correcto

    | Si necesitás... | Usá... | Porque... |
    |---|---|---|
    | Compartir rápido (WhatsApp, Classroom) | **MP3** | Archivo chico (3–8 MB por minuto), compatible con TODO |
    | Llevar a un estudio de grabación | **WAV** | Calidad máxima, sin compresión, estándar profesional |
    | Archivar con calidad pero sin ocupar tanto | **FLAC** | Misma calidad que WAV, ocupa la mitad |
    | Publicar en web con buena calidad | **OGG** | Alternativa libre al MP3, buena calidad/tamaño |

    #### 2. Configurar el MP3

    - **Bitrate (tasa de bits)**: 
      - **128 kbps**: aceptable para un demo rápido.
      - **192 kbps**: buena calidad para compartir.
      - **256 kbps**: muy buena calidad para música con matices.
      - **320 kbps**: máxima calidad MP3. Para entregas importantes.
    - **Recomendación para este curso**: 256 kbps mínimo.

    #### 3. Sample rate y normalización

    - **Sample rate**: 44100 Hz (estándar CD). No lo cambies a menos que sepas exactamente lo que hacés.
    - **Normalizar**: **ACTIVAR SIEMPRE**. Ajusta el volumen para que el pasaje más fuerte no distorsione y los más suaves se escuchen. Si no normalizás, tu MP3 puede sonar MUY BAJO.

    !!! warning "¿Qué pasa si NO normalizo?"
        Sin normalización: la parte más fuerte de tu obra está a −6 dB. Al reproducirla al lado de cualquier otra canción (normalizada a 0 dB), tu obra suena BAJÍSIMA. El oyente sube el volumen. Después tu obra termina y suena la siguiente canción... a TODO VOLUMEN. Eso es una mala experiencia. Normalizá SIEMPRE.

    #### 4. Rango de exportación

    Podés exportar la partitura COMPLETA o solo un fragmento seleccionando compases específicos. Esto es útil para:
    - Mandar un "extracto" sin tener que exportar 10 minutos de música.
    - Crear un "preview" de 30 segundos para redes sociales.

???+ note "Exportación masiva (batch export)"

    Si tenés una partitura con 8 instrumentos y necesitás exportar TODAS las partes como PDF + TODAS como MP3, ¿vas a hacer Archivo → Exportar 16 veces?

    **No. Usá la exportación masiva.**

    ### Exportar todas las partes como PDF

    1. **Archivo → Exportar → Exportar partes**.
    2. Seleccionar **PDF** como formato.
    3. Marcar las partes que querés exportar (o "Seleccionar todas").
    4. Elegir carpeta de destino.
    5. Clic en **Exportar**.

    MuseScore exporta TODAS las partes en UNA sola operación. Los archivos se nombran automáticamente con el nombre de cada parte.

    ### Exportar todo como MP3

    1. **Archivo → Exportar → Exportar partes**.
    2. Seleccionar **MP3** como formato.
    3. Configurar bitrate, sample rate y normalización.
    4. Seleccionar partes y carpeta.
    5. Clic en **Exportar**.

    ⚠️ **Paciencia**: exportar audio de 8 partes toma TIEMPO. Cada parte se "reproduce" internamente para generar el audio. 8 partes × 3 minutos = ~24 minutos de renderizado interno. No es que tu computadora es lenta: es que MuseScore está simulando una orquesta en tiempo real, 8 veces.

    !!! tip "Optimizar la exportación masiva de audio"
        - Cerrá otros programas para liberar recursos.
        - Si solo necesitás audio de ALGUNAS partes, no exportes TODAS.
        - Podés exportar las partes más importantes primero y el resto después.

???+ note "El árbol de decisión de formatos"

    Cada vez que terminás una partitura, preguntate:

    ```
    ¿Qué necesito hacer con mi partitura?
    │
    ├─ ¿Seguir editando YO?
    │  └─ Guardar como .mscz (Archivo → Guardar)
    │
    ├─ ¿Que otra persona EDITE en otro programa?
    │  └─ Exportar como .mxl (MusicXML comprimido)
    │
    ├─ ¿Que alguien LEA o IMPRIMA?
    │  └─ Exportar como .pdf
    │
    ├─ ¿Que alguien ESCUCHE?
    │  ├─ Calidad profesional → .wav o .flac
    │  └─ Compartir rápido → .mp3 (256+ kbps, normalizado)
    │
    ├─ ¿Poner en una página web, presentación o red social?
    │  ├─ Necesito que escale sin pixelarse → .svg
    │  └─ Tamaño fijo, solo para ver → .png (300 DPI)
    │
    └─ ¿Llevar a un DAW para producción musical?
       └─ Exportar como .mid (y después asignar sonidos VST en el DAW)
    ```

    > Insertar diagrama de flujo visual con el árbol de decisión.

???+ note "Metadatos: la información invisible que VIAJA con tu archivo"

    Cuando exportás un PDF o un MP3, el archivo contiene información INVISIBLE:
    - **Título** de la obra.
    - **Compositor** (vos).
    - **Copyright** (quién posee los derechos).
    - **Fecha** de creación.

    ### Cómo completar los metadatos

    1. **Archivo → Propiedades de la partitura**.
    2. Completar los campos:
       - **Título de la obra**: ej. "Serenata en Sol mayor"
       - **Compositor**: TU NOMBRE.
       - **Letrista**: solo si tiene letra.
       - **Copyright**: ej. "© 2026 José Urgilés. Todos los derechos reservados."
       - **Fuente**: si es un arreglo de una obra existente, acreditá al compositor original.

    ### ¿Por qué importan los metadatos?

    - Un PDF sin metadatos aparece como "Untitled" en cualquier visor.
    - Un MP3 sin metadatos aparece como "Unknown Artist" en cualquier reproductor.
    - Si tu obra circula por internet sin metadatos, NADIE sabe que es tuya.
    - Los metadatos son tu FIRMA DIGITAL. Completalos. Siempre.

    !!! warning "Metadatos en el examen"
        En el examen final, los metadatos INCOMPLETOS restan puntos. Un PDF con título "Untitled" y compositor vacío es un PDF ANÓNIMO. No entregues archivos anónimos.

---

## Actividad en Classroom

### Tarea: S29 — Exportación y formatos de entrega

> **Material necesario**: el docente proporcionará el archivo `ejercicio_S29_exportacion.mscz`, una partitura para sexteto (Flauta, Clarinete en Si♭, Violín I, Violín II, Viola, Violonchelo) en Sol mayor (1 sostenido), 4/4, 56 compases, con título, compositor, marcas de ensayo (A–G), dinámicas variadas (pp a ff), 2 cambios de tempo, articulaciones, texto de expresión y partes YA generadas y formateadas profesionalmente (con pentagrama 7.5 mm, pausas multi-compás, saltos correctos y cues).

1. **Completar metadatos.** Abrí `ejercicio_S29_exportacion.mscz`:
    - **Archivo → Propiedades de la partitura**.
    - Completá: título, compositor (TU nombre), copyright (© [año] [Tu Nombre]), fuente (si es arreglo de obra existente).
    - Guardá el archivo (.mscz).

2. **Exportación individual — 7 formatos.** Exportá la partitura general en los siguientes formatos con ESTAS configuraciones específicas:
    - `.mscz` — guardar normal. Tu archivo de trabajo.
    - `.mxl` — Archivo → Exportar → MusicXML comprimido (.mxl).
    - `.mid` — Archivo → Exportar → MIDI (.mid).
    - `.pdf` — Archivo → Exportar → PDF. Verificar que se vea correcto.
    - `.png` — Archivo → Exportar → PNG. Configurar 300 DPI. Seleccionar "Todas las páginas".
    - `.svg` — Archivo → Exportar → SVG. Seleccionar "Todas las páginas".
    - `.mp3` — Archivo → Exportar → MP3. Configurar: 256 kbps, 44100 Hz, NORMALIZAR activado.
    - `.wav` — Archivo → Exportar → WAV. 44100 Hz, normalizado. (⚠️ Va a ocupar mucho: ~25–30 MB.)
    
    Nombrá los archivos: `APELLIDO_S29_sexteto.formato`.

3. **Exportación masiva de partes como PDF.** Usá la exportación masiva:
    - **Archivo → Exportar → Exportar partes**.
    - Formato: PDF.
    - Seleccionar TODAS las partes (6 partes).
    - Exportar a una carpeta.
    - Los archivos deben nombrarse automáticamente con el nombre de cada instrumento.

4. **Prueba de roundtrip y pérdida.** Realizá el ciclo completo:
    - Exportá la partitura como `.mxl` (si ya lo hiciste en el paso 2, usá ese archivo).
    - **Reimportalo** en MuseScore: Archivo → Abrir → seleccionar tu `.mxl`.
    - Compará la versión reimportada con la original (solapá las ventanas).
    - **Documentá las diferencias**: creá una tabla con al menos 5 cosas que CAMBIARON entre la original y la reimportada (ej. "fuente del título cambió", "los saltos de página desaparecieron", "las posiciones de las dinámicas se movieron").

5. **"Paquete para el estudio de grabación".** Simulá que un estudio de grabación te pidió tu obra para producirla profesionalmente. Prepará un paquete comprimido (ZIP) que contenga:
    - `.wav` de la partitura completa (máxima calidad).
    - `.mid` con todos los instrumentos (para cargar en el DAW).
    - `.mxl` de la partitura general (por si necesitan editar algo).
    - `.pdf` de la partitura general (para que el productor lea).
    - `.pdf` de CADA parte individual (6 PDFs, por si graban músicos reales).
    - Comprimí todo en `APELLIDO_S29_estudio.zip`.

6. **Árbol de decisión personalizado.** Creá tu propio árbol de decisión (como el de la sección "El árbol de decisión de formatos") pero para TU contexto musical. Si tocás guitarra, adaptalo a situaciones de guitarrista. Si tocás piano, adaptalo. Si componés para orquesta, adaptalo. Dibujalo o escribilo en texto en tu comentario de Classroom.

7. **Reflexión sobre formatos.** En Classroom, respondé:
    - ¿Cuál fue el formato que MÁS te sorprendió por lo que pierde o gana? ¿Por qué?
    - De los 7 formatos que exportaste, ¿cuál usarías en CADA UNA de estas situaciones? Justificá cada elección.
        - (a) Mandar la partitura por WhatsApp a un amigo que usa Finale.
        - (b) Publicar un fragmento de tu obra en Instagram.
        - (c) Entregar la partitura a un jurado para un concurso de composición.
        - (d) Archivar tu obra para dentro de 20 años (backup definitivo).
    - ¿Cuánto pesa el archivo .wav comparado con el .mp3? ¿Cuánto pesa el .mscz comparado con el .mxl? ¿Qué aprendiste sobre el costo del "tamaño" vs. la "calidad"?

### Entregables

- [ ] Archivo `.mscz` con metadatos completos
- [ ] `.mxl` (MusicXML comprimido)
- [ ] `.mid` (MIDI)
- [ ] `.pdf` (partitura general)
- [ ] `.png` (300 DPI, todas las páginas)
- [ ] `.svg` (todas las páginas)
- [ ] `.mp3` (256 kbps, normalizado)
- [ ] `.wav` (44100 Hz, normalizado)
- [ ] Carpeta con 6 PDFs de las partes individuales (exportación masiva)
- [ ] `APELLIDO_S29_estudio.zip` (paquete para estudio de grabación)
- [ ] Comentario en Classroom con: (a) tabla de roundtrip (≥5 diferencias entre original y reimportado), (b) árbol de decisión personalizado, (c) respuestas a las 3 preguntas de reflexión.

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Metadatos | Título, compositor, copyright y fuente completos | 3 de 4 completos | ≤2 completos |
| Formatos individuales | 7 formatos exportados con configuraciones correctas (MP3 256k normalizado, PNG 300 DPI, etc.) | 5–6 formatos correctos | ≤4 formatos |
| Batch export (PDF) | 6 partes exportadas en una operación; archivos con nombre de instrumento | 4–5 partes exportadas | ≤3 partes |
| Roundtrip y tabla de pérdidas | .mxl exportado y reimportado; tabla con ≥5 diferencias documentadas | Reimportado pero tabla con 3–4 diferencias | Sin roundtrip |
| Paquete de estudio | ZIP con .wav + .mid + .mxl + .pdf (score) + 6 PDFs (partes) | Faltan 1–2 archivos | Faltan ≥3 archivos |
| Árbol de decisión y reflexión | Árbol personalizado coherente; 3 respuestas con criterio técnico | 2 de 3 correctas | ≤1 respuesta correcta |

---

*Basado en: MuseScore Studio 4 Handbook — Basics: Open/Save/Export/Print | Advanced topics: File formats | https://handbook.musescore.org*
