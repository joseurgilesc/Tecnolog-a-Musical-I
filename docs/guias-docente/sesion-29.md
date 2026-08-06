# Guía Docente — Sesión 29: Exportación y formatos de entrega

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivo `ejercicio_S29_exportacion.mscz` (partitura con partes para exportación multiformato)  
**Referencia:** MuseScore Studio Handbook — Basics: Open/Save/Export/Print, Advanced topics: File formats

---

## Objetivo de la sesión

Que el estudiante domine el ecosistema completo de formatos de archivo en MuseScore y tome decisiones informadas sobre qué formato usar en cada situación profesional: archivos nativos de trabajo (.mscz), formatos de intercambio entre editores (MusicXML .mxl), formatos de audio para distribución (.mp3, .wav, .flac), formatos gráficos para integración en documentos (.pdf, .png, .svg), y formatos de intercambio para DAWs (.mid). El estudiante debe entender las VENTAJAS y PÉRDIDAS de cada formato y saber ejecutar exportaciones masivas (batch export) de partes con configuración profesional.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S28 + pregunta disparadora: "Te pidieron la partitura para publicar en una revista, para un ensayo y para Instagram. ¿Mandás lo mismo?" |
| **Desarrollo** | 30 min | Demostración: exportación en 8 formatos → análisis de pérdidas por formato → configuración de audio → exportación masiva |
| **Práctica** | 65 min | Árbol de decisión de formatos, exportación completa con configuraciones, tabla comparativa de formatos |
| **Cierre** | 15 min | Revisión de tabla de formatos, casos prácticos de decisión, entrega |

---

## 1. Apertura — Un archivo, muchas caras

### Materiales
- Proyector con MuseScore Studio abierto.
- Archivo `ejercicio_S29_exportacion.mscz` publicado en Classroom **antes de la clase**.
- Opcional: tener abiertos otros programas (navegador con Google Drive, Vista Previa de PDF, reproductor de audio) para mostrar cada formato en su contexto real.

### Dinámica

1. **Revisión de S28** (4 min):
   - ¿Cuánto tiempo les llevó formatear TODAS las partes? ¿Más o menos del que esperaban?
   - ¿Cuál fue el error más "invisible" que encontraron en las partes sucias?

2. **Preguntas disparadoras** (6 min):
   - Plantear el escenario: "Terminaste tu obra. La escribiste en MuseScore. Generaste las partes. Todo está perfecto. Ahora... TRES personas te piden el archivo:"
     - "Tu profesor de composición: 'Mandame la partitura para corregirla.'"
     - "El director del ensamble: 'Mandame las partes en PDF para imprimir.'"
     - "Tu amigo productor: 'Mandame el audio para ponerlo en el demo.'"
   - "¿Le mandás el MISMO archivo a los tres?"
   - (Dejar que discutan. Generalmente responden "no", pero no saben exactamente qué mandar a cada uno.)
   - Proyectar la frase: **"Cada formato cuenta una historia diferente de tu misma música."**

---

## 2. Desarrollo — El ecosistema de formatos de MuseScore

### Secuencia sugerida

1. **Los 8 formatos en 8 minutos** (8 min). Crear un diagrama en el pizarrón mientras se explica:

   | Formato | Tipo | ¿Para quién? | ¿Qué preserva? | ¿Qué PIERDE? |
   |---|---|---|---|---|
   | **.mscz** | Nativo (comprimido) | Para VOS | TODO (notas, formato, sonidos, historia de edición) | NADA (es tu backup perfecto) |
   | **.mscx** | Nativo (sin comprimir) | Para CONTROL de versiones (Git) | Todo, en XML legible | Ocupa mucho más espacio |
   | **.mxl** | Intercambio (comprimido) | Otro editor de partituras | Notas, ritmos, texto, dinámicas, marcas | Formato de página, fuentes, espaciado exacto |
   | **.musicxml** | Intercambio (sin comprimir) | Procesamiento automático | Igual que .mxl | Igual que .mxl, pero archivo enorme |
   | **.mid** | Secuenciación | DAWs (Ableton, Logic, Reaper) | Notas (altura + duración), tempo, programa | TODO lo visual, dinámicas como velocity, articulaciones como duración |
   | **.pdf** | Documento (vectorial) | Imprenta, atril, publicación | Apariencia visual EXACTA | No editable (sin software especializado) |
   | **.png** | Imagen (raster) | Web, redes sociales, documentos Word | Captura visual de la página | No editable, NO escalable (se pixela al ampliar) |
   | **.svg** | Imagen (vectorial) | Diseño gráfico, web escalable, Illustrator | Gráfico vectorial de la página | No es una partitura editable |
   | **.mp3** | Audio (comprimido) | Distribución general, streaming | Sonido aceptable | Calidad de audio (compresión con pérdida), metadatos limitados |
   | **.wav** | Audio (sin comprimir) | Producción profesional, mezcla, masterización | Sonido en máxima calidad | Archivos ENORMES |
   | **.flac** | Audio (comprimido sin pérdida) | Archivo de alta calidad, distribución audiófila | Sonido perfecto (mitad del tamaño de WAV) | No todos los reproductores lo soportan |

   - **Demostración rápida**: exportar la MISMA partitura en .pdf, .png y .svg. Mostrar los tres archivos lado a lado. "¿Ven la diferencia? El PDF es nítido a cualquier zoom. El PNG se pixela. El SVG se ve perfecto pero NO es una partitura: es un dibujo."

2. **Configuración de exportación de audio** (8 min):
   - "Exportar audio NO es solo 'Archivo → Exportar → MP3'. Hay decisiones que afectan la calidad."
   - Abrir el diálogo de exportación de audio.
   - **Formato**: MP3 (distribución) vs. WAV (producción) vs. FLAC (archivo).
     - "MP3: para mandar por WhatsApp o publicar en Classroom. Archivo chico, calidad aceptable."
     - "WAV: para llevar a un estudio de grabación. Calidad máxima. Archivo GIGANTE."
     - "FLAC: lo mejor de ambos mundos. Calidad de WAV, tamaño de MP3×3. Pero no todos los programas lo leen."
   - **Bitrate (MP3)**: 128 kbps (aceptable), 192 kbps (bueno), 256 kbps (muy bueno), 320 kbps (máximo). "Para música clásica o partituras con mucho detalle dinámico, usá 256 o 320. Para un demo rápido, 128 alcanza."
   - **Sample rate**: 44100 Hz (estándar CD). "MuseScore por defecto usa 44100. No lo cambies a menos que sepas exactamente por qué."
   - **Normalizar**: "Activar SIEMPRE. Ajusta el volumen para que el punto más fuerte de la pieza no distorsione. Si no normalizás, tu MP3 puede sonar bajísimo."
   - **Rango de exportación**: "Podés exportar solo un fragmento (compases 1–16) o la partitura completa. Útil para mandar un extracto sin tener que exportar 10 minutos de música."

3. **Exportación masiva (batch export)** (5 min):
   - "Si tenés una partitura con 8 instrumentos y necesitás exportar todas las partes como PDF + todas como MP3, ¿vas a hacer Archivo → Exportar 16 veces?"
   - Mostrar: **Archivo → Exportar → Exportar partes**.
   - Seleccionar formato (PDF). "MuseScore exporta TODAS las partes en UNA sola operación."
   - "Pero OJO: solo podés elegir UN formato por vez. Si querés PDF Y MP3, tenés que hacer dos exportaciones masivas."
   - Mostrar también `Archivo → Exportar → Exportar` para la partitura completa vs. partes individuales.

4. **El árbol de decisión de formatos** (4 min). Dibujar en el pizarrón:

   ```
   ¿Qué necesito hacer con mi partitura?
   │
   ├─ ¿Seguir editando YO?
   │  └─ .mscz (guardar normal)
   │
   ├─ ¿Que otra persona EDITE en otro programa?
   │  └─ .mxl (MusicXML comprimido)
   │
   ├─ ¿Que alguien LEA o IMPRIMA?
   │  └─ .pdf
   │
   ├─ ¿Que alguien ESCUCHE?
   │  ├─ Calidad profesional → .wav o .flac
   │  └─ Compartir rápido → .mp3 (256+ kbps)
   │
   ├─ ¿Poner en una página web o presentación?
   │  ├─ Necesito escalar → .svg
   │  └─ Tamaño fijo → .png
   │
   └─ ¿Llevar a un DAW para producción?
      └─ .mid (y después ajustás sonidos en el DAW)
   ```

5. **Metadatos: la información invisible** (5 min):
   - "Cuando exportás un PDF o un MP3, el archivo lleva metadatos: título, autor, copyright."
   - Mostrar cómo configurarlos: **Archivo → Propiedades de la partitura → Metadatos**.
   - "Si no completás los metadatos, tu PDF va a decir 'Untitled' y tu MP3 'Unknown Artist'. En el mundo profesional, eso es IMPERDONABLE."
   - Campos importantes: Título de la obra, Compositor, Arreglista (si aplica), Copyright, Fuente (si es arreglo de otra obra).

---

## 3. Práctica — El laboratorio de formatos

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S29 — Exportación y formatos de entrega

**Material**: el docente proporciona el archivo `ejercicio_S29_exportacion.mscz`:
   - Partitura para sexteto (Flauta, Clarinete en Si♭, Violín I, Violín II, Viola, Violonchelo) en Sol mayor (1 sostenido), 4/4, 56 compases.
   - Debe incluir título, compositor, marcas de ensayo (A–G), dinámicas variadas (pp a ff), cambios de tempo (mínimo 2), articulaciones, texto de expresión.
   - Las partes deben estar YA generadas y formateadas (tamaño 7.5 mm, pausas multi-compás, saltos de página correctos, cues en silencios de +8 compases).
   - El objetivo NO es generar partes (eso fue S28), sino EXPORTARLAS en múltiples formatos con decisiones informadas.

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Completar metadatos profesionales.
2. Exportar en 7 formatos distintos con configuraciones específicas.
3. Exportación masiva de partes como PDF.
4. Comparación de pérdidas: MSCZ → MXL → reimportar.
5. Árbol de decisión personalizado.
6. Archivo "para el estudio de grabación" con requisitos profesionales.
7. Reflexión sobre formatos y contexto.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Metadatos | Título, compositor, copyright y fuente completos | 3 de 4 completos | ≤2 completos |
| Exportación individual (7 formatos) | .mscz, .mxl, .mid, .pdf, .png, .svg, .mp3 exportados con configuraciones correctas | 5–6 formatos correctos | ≤4 formatos |
| Configuración de audio | MP3 a 256+ kbps, normalizado, sample rate 44100 | Configuración parcialmente correcta | Sin normalizar o bitrate bajo |
| Batch export (PDF) | 6 partes exportadas en una operación; archivos con nombres de instrumento | 4–5 partes exportadas | ≤3 partes |
| Roundtrip MXL | MusicXML exportado y reimportado; tabla con pérdidas documentadas (≥5 diferencias) | Reimportado pero tabla incompleta | Sin roundtrip |
| "Estudio de grabación" | .wav + .mid + .mxl en carpeta comprimida; nivel profesional | Archivos presentes pero incompletos | Faltan formatos clave |
| Reflexión | 3 respuestas con comprensión de pérdidas y contexto de uso | 2 respuestas correctas | ≤1 respuesta |

---

## 4. Cierre — El formato correcto para la persona correcta

### Revisión por parejas (8 min)

- Intercambiar la tabla de roundtrip MXL: "¿Tu compañero encontró las mismas pérdidas que vos? ¿Hay algo que vos perdiste y él no?"
- Intercambiar el ZIP "estudio de grabación": "Si fueras el ingeniero de sonido, ¿podrías trabajar con estos archivos? ¿Qué falta?"

### Puesta en común (7 min)

- "Levanten la mano: ¿cuál fue la pérdida más SORPRENDENTE en el roundtrip MXL?" (Discusión: formato de página, tipos de letra, posición de marcas.)
- "Escenario rápido: tenés 10 segundos para decidir. Te mandan un WhatsApp: 'Che, pasame la partitura'. ¿Qué formato mandás?" (Discusión: ¿.pdf o .mxl? Depende de si la persona va a leer o editar.)
- "¿Alguien exportó en .wav y se asustó con el tamaño del archivo?" → "Bienvenidos al mundo de audio profesional. Un WAV de 3 minutos puede ocupar 30 MB. Por eso el MP3 existe."

### Resumen del docente (5 min)

1. **No existe UN formato perfecto.** Cada formato sacrifica algo para ganar en otra cosa. El .mscz lo guarda TODO pero solo lo abre MuseScore. El .mp3 lo escucha cualquiera pero perdió calidad. El .pdf se ve perfecto pero no se edita. La madurez profesional es saber ELEGIR.

2. **MusicXML es el puente, pero es un puente IMPERFECTO.** Vas a perder formato de página, fuentes, espaciado exacto. Saber QUÉ se pierde te permite anticiparte y compensar.

3. **Los metadatos NO son opcionales.** En el mundo profesional, un archivo sin metadatos es un archivo ANÓNIMO. Si querés que te reconozcan como el autor de tu obra, poné tu nombre en los metadatos. Siempre.

4. **Exportación masiva: ahorrá tiempo, no calidad.** El batch export de MuseScore es potente. Pero solo funciona si REVISASTE cada parte individualmente ANTES. Exportar 20 PDFs en 2 segundos es fácil. Revisar que los 20 PDFs estén bien formateados es lo que toma tiempo.

5. **El audio exportado de MuseScore NO es una producción final.** Es un demo de alta calidad. Los sonidos de MuseScore son buenos, pero no reemplazan una orquesta real ni samples profesionales. Si llevás tu .wav a un estudio, el ingeniero va a apreciar que esté normalizado y a 44100 Hz. Pero probablemente lo use como referencia, no como pista final.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| La exportación a MP3 no produce audio (silencio) | Verificar que la reproducción funcione DENTRO de MuseScore. Si dentro suena: revisar ruta de exportación, permisos de escritura. Si dentro NO suena: problema de sintetizador (Preferences → Audio/MIDI). |
| El PDF exportado tiene las partes en orden alfabético, no en orden de partitura | En el diálogo "Exportar partes", las partes se listan en el orden en que aparecen en la partitura. Si están desordenadas, reorganizalas en el diálogo de Partes (Archivo → Partes) antes de exportar. |
| El estudiante exporta un .mid y al abrirlo en un DAW suena "mal" (piano para todos los instrumentos) | El MIDI no contiene sonidos, solo números de programa (program change). Explicar que en el DAW debe asignar instrumentos virtuales (VST) a cada canal MIDI. El MIDI es una "partitura para sintetizadores", no audio. |
| El .png exportado se ve pixelado o borroso | La resolución del PNG se configura en el diálogo de exportación. Aumentar DPI (dots per inch) a 300 para impresión o 150 para web. El valor por defecto (150) es aceptable para pantalla pero bajo para impresión. |
| El .svg exportado se ve diferente al abrirlo en Illustrator/Inkscape | Las fuentes musicales (Bravura, Leland) son fuentes especializadas. Si el programa de diseño no las tiene instaladas, usará una fuente de sustitución y la partitura se verá rota. Solución: instalar las fuentes de MuseScore en el sistema, o convertir el texto a curvas antes de exportar. |
| El estudiante confunde .mscz (nativo) con .mscx (nativo sin comprimir) | .mscz es un ZIP que contiene el .mscx + imágenes + fuentes. .mscx es el XML solo. Para trabajo diario: .mscz. Para Git/control de versiones: .mscx (porque Git puede hacer diff de XML pero no de binarios ZIP). |
| La exportación masiva de partes como MP3 tarda muchísimo | Es normal. Cada parte se "reproduce" internamente para generar el audio. 8 partes × 3 minutos = 24 minutos de renderizado interno. Recomendar exportar las partes más importantes primero y dejar las demás para después si el tiempo es limitado. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — File formats](https://handbook.musescore.org/advanced-topics/file-formats.md)
- [MuseScore Studio Handbook — Open/Save/Export/Print](https://handbook.musescore.org/basics/save-export-print.md)
- **Preparación del archivo `ejercicio_S29_exportacion.mscz`**: crear sexteto en Sol mayor, 4/4, 56 compases. Completar la partitura con material musical rico (todas las voces con movimiento independiente). Incluir título ("Serenata en Sol"), compositor (nombre ficticio), marcas de ensayo A–G, dinámicas pp a ff, al menos 2 cambios de tempo (ej. Andante → Allegro), articulaciones (staccato, acentos, tenuto), texto de expresión (dolce, espressivo, con fuoco). Generar TODAS las partes y formatearlas profesionalmente (7.5 mm, pausas multi-compás, saltos de página, cues). El archivo debe ser el punto de partida perfecto para la práctica de exportación.
- Dato curioso: el formato MP3 fue desarrollado en 1993 por el Instituto Fraunhofer de Alemania. Usa un modelo psicoacústico: elimina frecuencias que el oído humano "no escucha" (enmascaradas por sonidos más fuertes). Es técnicamente una "partitura con pérdida" del audio. Para una partitura de cuerdas con muchos armónicos, el MP3 puede eliminar frecuencias que SÍ son audibles para un músico entrenado. Por eso en contextos profesionales se prefiere WAV o FLAC.
- Dato curioso: el formato PDF fue creado por Adobe en 1993 como un "sobre digital": un archivo que se ve EXACTAMENTE igual en cualquier computadora, independientemente del sistema operativo o las fuentes instaladas. Esa es la razón por la que es el estándar para partituras: cuando imprimís un PDF, lo que ves es lo que obtenés. En MuseScore, cuando exportás a PDF, el programa internamente "imprime" la partitura en un archivo en lugar de en papel.
- Ejercicio opcional de ampliación: crear una partitura de 1 página. Exportarla en .pdf, .png (150 DPI), .png (300 DPI), .svg y .musicxml. Abrir los 5 archivos y compararlos visualmente. Escribir un breve informe sobre qué formato elegirías para: (a) enviar a una imprenta profesional, (b) publicar en una red social, (c) insertar en un documento de Word, (d) enviar a un colega que usa Sibelius, (e) archivar para la posteridad.

---

*Guía docente — Tecnología Musical I | Sesión 29*
