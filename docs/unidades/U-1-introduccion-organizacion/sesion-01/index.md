# Sesión 1: Presentación e instalación de MuseScore

📚 Handbook → Getting Started — Download and Installation, Learning MuseScore | Herramientas: MuseScore Studio 4, Google Classroom, explorador de archivos

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término o formato que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="mscz"></a> **MSCZ** | Formato nativo y editable de MuseScore. Contiene toda la información de la partitura: notas, estilos, diseño. Es al archivo `.mscz` lo que un `.docx` al procesador de texto. |
    | <a id="pdf"></a> **PDF** | Formato de documento portátil. Se usa para distribuir e imprimir partituras. No es editable en MuseScore una vez exportado. |
    | <a id="musicxml"></a> **MusicXML** | Formato de intercambio estándar entre editores de partituras (MuseScore, Sibelius, Finale, Dorico). Conserva información musical, no solo visual. |
    | <a id="midi"></a> **MIDI** | Protocolo y formato que almacena instrucciones de ejecución (nota, duración, velocidad), no audio. Permite importar y exportar datos entre MuseScore, DAWs e instrumentos. |
    | <a id="paleta"></a> **Paleta** | Panel lateral de MuseScore que agrupa símbolos musicales por categoría: claves, armaduras, dinámicas, articulaciones, líneas, etc. Se arrastran a la partitura. |
    | <a id="panel-propiedades"></a> **Panel de propiedades** | Panel contextual que muestra y permite editar los atributos del elemento seleccionado: posición, visibilidad, color, estilo. |
    | <a id="mezclador"></a> **Mezclador** | Panel que controla el volumen, panorama, silencio y solo de cada instrumento durante la reproducción. Equivalente a un mezclador de audio virtual. |
    | <a id="interfaz"></a> **Interfaz** | Conjunto de ventanas, barras, menús y paneles que componen el entorno visual de MuseScore Studio. Incluye la barra de herramientas, el área de partitura, las paletas y los paneles. |

???+ note "La notación musical digital dentro de la práctica profesional"

    La escritura musical digital no es un complemento optativo: es parte del flujo de trabajo profesional contemporáneo. Un compositor, arreglista, director o educador musical necesita producir partituras que sean:

    - **Legibles**: con espaciado, paginación y distribución instrumental adecuados.
    - **Editables**: que permitan correcciones, transposiciones y extracción de partes sin rehacer el trabajo.
    - **Intercambiables**: capaces de abrirse en otros programas, enviarse a colegas o importarse desde otras fuentes.
    - **Publicables**: listas para imprimir, exportar a PDF o compartir en plataformas digitales.

    MuseScore Studio ocupa un lugar particular en este ecosistema: es un editor de partituras profesional, gratuito y de código abierto, con una comunidad activa que produce tutoriales, plantillas y mejoras continuas.

    | Necesidad profesional | Herramienta en MuseScore |
    |---|---|
    | Escribir para orquesta, banda o coro | Creación de score con múltiples instrumentos |
    | Compartir con colegas que usan Sibelius o Finale | Exportación e importación [MusicXML](#musicxml) |
    | Entregar una partitura lista para imprimir | Exportación a [PDF](#pdf) |
    | Escuchar cómo suena la obra antes de ensayar | Reproducción integrada con biblioteca de sonidos |
    | Extraer la parte de cada músico | Generación automática de particellas |
    | Trabajar con un DAW o instrumento virtual | Exportación e importación [MIDI](#midi) |


???+ note "Instalación y configuración inicial"

    ### Descarga e instalación

    MuseScore Studio está disponible para Windows, macOS y Linux. El instalador se descarga desde [musescore.org](https://musescore.org).


    <iframe width="100%" height="400" src="https://www.youtube.com/embed/grKX-cBEEmM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="border-radius: 8px; margin: 12px 0;"></iframe>

    Durante la instalación, el programa ofrece crear una cuenta opcional en MuseScore.com. Esta cuenta permite sincronizar partituras en la nube y publicar en la comunidad, pero **no es necesaria** para trabajar localmente. El curso se enfoca en el trabajo con archivos locales.

    ### Configuración de idioma

    MuseScore Studio permite cambiar el idioma de la interfaz desde **Editar → Preferencias → General** (o **Edit → Preferences → General**). Se recomienda usar la interfaz en español durante el curso para familiarizarse con la terminología en ambos idiomas.

    ### Configuración de audio y MIDI

    Desde **Editar → Preferencias → Audio y MIDI**, se puede seleccionar:
    - El dispositivo de salida de audio (altavoces internos, interfaz de audio, audífonos).
    - El dispositivo de entrada MIDI, si se dispone de un teclado o controlador conectado.

    Para las primeras sesiones, basta con verificar que el audio funciona correctamente. La conexión MIDI se abordará más adelante (Unidad 6).

    ### Verificación rápida

    Al abrir MuseScore Studio por primera vez, la pantalla de **Inicio** muestra:
    - **Nueva partitura**: asistente paso a paso para crear un score.
    - **Abrir**: explorador para localizar archivos [.mscz](#mscz), [MusicXML](#musicxml) o [MIDI](#midi).
    - **Partituras recientes**: acceso rápido a los últimos archivos trabajados.
    - **Plantillas**: scores preconfigurados por tipo de ensamble.

???+ note "Formatos de archivo: MSCZ, PDF, MusicXML, MIDI, imagen y audio"

    MuseScore trabaja con el formato nativo [MSCZ](#mscz), pero también lee y escribe otros formatos. Cada uno tiene un propósito distinto en el flujo de trabajo:

    | Formato | Tipo | ¿Editable? | ¿Para qué se usa? |
    |---|---|---|---|
    | **MSCZ** | Nativo (comprimido) | Sí | Archivo de trabajo principal. Conserva todo: notas, estilo, diseño, historial de deshacer. |
    | **MSCX** | Nativo (sin comprimir) | Sí | Variante sin compresión. Útil para control de versiones con Git o edición manual del XML. |
    | **PDF** | Documento | No | Impresión, distribución, entrega final. El estándar para partituras profesionales. |
    | **MusicXML** | Intercambio | Sí (al importar) | Transferir partituras entre MuseScore, Sibelius, Finale, Dorico y otros editores. |
    | **MIDI** | Datos de ejecución | Limitada | Importar desde un DAW o teclado; exportar para usar sonidos externos. Pierde información de notación. |
    | **PNG / SVG** | Imagen | No | Insertar fragmentos de partitura en documentos, presentaciones o sitios web. |
    | **Audio (WAV, MP3, FLAC)** | Sonido | No | Generar una referencia sonora de la partitura para compartir sin necesidad de MuseScore. |

    !!! warning "MIDI no es notación"
        Un archivo MIDI almacena qué nota se toca, cuándo y con qué intensidad, pero **no** contiene información sobre cómo debe verse en el pentagrama: no incluye articulaciones, dinámicas escritas, texto, ni decisiones de enharmonía. Importar un MIDI produce una partitura aproximada que requiere edición manual para ser publicable.

???+ note "Organización de carpetas, nombres de archivo y versiones"

    La organización del espacio de trabajo es una competencia profesional subestimada. Un músico que entrega archivos con nombres como `partitura_final_version_3_corregida_real.mscz` está comunicando desorden. La convención propuesta para este curso es:

    ### Estructura de carpetas

    ```
    TecnologiaMusicalI/
    ├── ejercicios/        ← ejercicios de clase, uno por sesión
    │   ├── S01/
    │   ├── S02/
    │   └── ...
    ├── evaluaciones/      ← exámenes y trabajos calificados
    ├── recursos/          ← partituras de referencia, PDFs, archivos MIDI fuente
    ├── exportaciones/     ← PDFs, PNGs, archivos de audio generados
    └── respaldos/         ← copias de seguridad periódicas
    ```

    ### Convención de nombres

    ```
    APELLIDO_Nombre_SesionNN_Descripcion_v01.mscz
    APELLIDO_Nombre_SesionNN_Descripcion_v01.pdf
    ```

    **Ejemplo**: `URGILES_Jose_S01_Instalacion_v01.mscz`

    - El número de versión (`v01`, `v02`) avanza con cada corrección significativa.
    - Nunca uses palabras como "final", "definitivo" o "corregido" en el nombre del archivo: la versión lo dice todo.
    - Evitá espacios y caracteres especiales en los nombres de archivo.

---

## Actividad en Classroom

### Tarea: S01 — Instalación, verificación y organización

1. **Instalá o verificá MuseScore Studio** en tu computador personal. Si usás un equipo del laboratorio, confirmá que la aplicación abre correctamente.
2. **Configurá el idioma** de la interfaz y comprobá que el audio funciona: abrí una partitura de demo desde la pantalla de Inicio y reproducila.
3. **Creá la estructura de carpetas** descrita arriba dentro de una carpeta principal llamada `TecnologiaMusicalI`.
4. **Capturá la pantalla** de MuseScore Studio abierto con una partitura de demo cargada y el panel de reproducción visible.
5. **Escribí una breve reflexión** (5–8 líneas) sobre dos usos concretos — académicos o profesionales — que le darías a MuseScore en tu carrera.

### Entregables

- [ ] Captura de pantalla de MuseScore Studio funcionando (PNG o JPG)
- [ ] Reflexión escrita (PDF o texto en el mismo Classroom)
- [ ] Ambas cosas organizadas con el formato de nombre: `APELLIDO_Nombre_S01_Instalacion_v01`

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Instalación y audio | MuseScore abre y reproduce sonido sin errores | Abre pero no reproduce audio | No abre o no se instaló |
| Organización de carpetas | Las 5 carpetas existen con los nombres indicados | Faltan 1–2 carpetas | No se creó la estructura |
| Reflexión | Menciona ≥2 usos concretos con contexto profesional | Menciona 1 uso o ideas vagas | No entrega reflexión |
| Nombres de archivo | Sigue la convención `APELLIDO_Nombre_S01_*_v01` | Se aproxima pero tiene errores | No sigue la convención |

---

*Basado en: MuseScore 3 Handbook — Getting Started: Download and Installation, Learning MuseScore | https://musescore.org/en/handbook/3*
