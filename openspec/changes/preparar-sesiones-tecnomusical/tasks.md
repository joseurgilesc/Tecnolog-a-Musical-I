# Tasks: Preparar Sesiones Tecnomusical

## Tabla de Resumen

| Batch | Sesiones | Archivos | Est. Líneas | Excede 400? |
|-------|----------|----------|-------------|-------------|
| 0 | — | — | 0 | — (verificación) |
| 1 | 1, 2, 3 | 3 index + 3 guías | ~660 | **Sí** |
| 2 | 4, 5 | 2 index + 2 guías | ~440 | **Sí** |
| 3 | 6, 7, 8 | 3 index + 3 guías | ~660 | **Sí** |
| 4 | 9, 10 | 2 index + 2 guías | ~440 | **Sí** |
| 5 | 11, 12 | 2 index + 2 guías | ~480 | **Sí** |
| 6 | 13, 14 | 2 index + 2 guías | ~480 | **Sí** |
| 7 | 15, 16 | 1 index + 1 guía + 1 examen | ~320 | No |
| 8 | 17, 18, 19 | 3 index + 3 guías | ~720 | **Sí** |
| 9 | 20, 21 | 2 index + 2 guías | ~480 | **Sí** |
| 10 | 22, 23, 24 | 3 index + 3 guías | ~720 | **Sí** |
| 11 | 25, 26, 27 | 3 index + 3 guías | ~720 | **Sí** |
| 12 | 28, 29, 30, 31, 32 | 4 index + 4 guías + 1 examen | ~1,010 | **Sí** |
| 13 | — | — | 0 | — (verificación) |
| **Total** | **31 + 2 exam** | **65 archivos** | **~7,130** | 11/12 batches |

---

## Review Workload Forecast

| Field | Value |
|-------|-------|
| Estimated changed lines | ~7,130 |
| 400-line budget risk | Medium |
| Chained PRs recommended | Yes (user accepted: per-batch delivery) |
| Suggested split | 12 stacked PRs → main |
| Delivery strategy | auto-chain (force-chained, size:exception accepted) |
| Chain strategy | stacked-to-main |

Decision needed before apply: No
Chained PRs recommended: Yes
Chain strategy: stacked-to-main
400-line budget risk: Medium
Size exception: user-authorized (per-batch del ivery)

### Suggested Work Units

| Unit | Goal | PR | Test | Rollback |
|------|------|-----|------|----------|
| B1 | Sessions 1-3 (U1: introducción) | PR 1 | `mkdocs build --strict` | `git revert` |
| B2 | Sessions 4-5 (U2: ingreso notas I) | PR 2 | `mkdocs build --strict` | `git revert` |
| B3 | Sessions 6-8 (U2: compases, métrica) | PR 3 | `mkdocs build --strict` | `git revert` |
| B4 | Sessions 9-10 (U3: articulaciones) | PR 4 | `mkdocs build --strict` | `git revert` |
| B5 | Sessions 11-12 (U3: líneas, voces) | PR 5 | `mkdocs build --strict` | `git revert` |
| B6 | Sessions 13-14 (U4: repeticiones) | PR 6 | `mkdocs build --strict` | `git revert` |
| B7 | Sessions 15-16 (integración + examen) | PR 7 | `mkdocs build --strict` | `git revert` |
| B8 | Sessions 17-19 (U5: acordes, percusión, piano) | PR 8 | `mkdocs build --strict` | `git revert` |
| B9 | Sessions 20-21 (U5: guitarra, transpositores) | PR 9 | `mkdocs build --strict` | `git revert` |
| B10 | Sessions 22-24 (U6: MIDI, MusicXML) | PR 10 | `mkdocs build --strict` | `git revert` |
| B11 | Sessions 25-27 (U6-U7: reproducción, formato) | PR 11 | `mkdocs build --strict` | `git revert` |
| B12 | Sessions 28-32 (U7: partes, exportación + examen final) | PR 12 | `mkdocs build --strict` | `git revert` |

---

## Batch 0: Verificación pre-aplicación

- [x] 0.1 Ejecutar `mkdocs build --strict` desde `/tmp/tecnomusical` — registrar errores existentes
- [x] 0.2 Verificar que todos los `sesion-{NN}/index.md` existen como placeholders (`<!-- Contenido pendiente -->`)
- [x] 0.3 Verificar que `docs/guias-docente/` existe (crear si no)
- [x] 0.4 Verificar que `mkdocs.yml` incluye todas las sesiones en el nav (7 unidades, 31 sesiones, 2 exámenes)
- [x] 0.5 Reportar: número de placeholders, estado del build, archivos faltantes
- **Dependencias**: Ninguna
- **Criterio**: Build actual documentado; lista de placeholders confirmada; directorio guias-docente creado

---

## Batch 1: Sesiones 1, 2, 3 — U1: Introducción y organización

- [x] 1.1 Crear `docs/unidades/U-1-introduccion-organizacion/sesion-01/index.md` — Handbook: Getting Started / Download and Installation, Basics / Viewing and navigation. Glosario ≤10 entradas (instalación, interfaz). Sin figuras pesadas. Header: "Presentación e instalación de MuseScore"
- [x] 1.2 Crear `docs/guias-docente/sesion-01.md` — Rúbrica 2 criterios, diagnóstico inicial, instalación guiada
- [x] 1.3 Crear `docs/unidades/U-1-introduccion-organizacion/sesion-02/index.md` — Handbook: Basics / Create new score, Instruments, Score properties. Figuras: asistente de nueva partitura, selector de instrumentos. Header: "Creación de una partitura nueva"
- [x] 1.4 Crear `docs/guias-docente/sesion-02.md` — Actividad: plantilla de ensamble, rúbrica 3 criterios
- [x] 1.5 Crear `docs/unidades/U-1-introduccion-organizacion/sesion-03/index.md` — Handbook: Basics / Viewing and navigation, Selection modes, Undo and redo. Figuras: modos de vista, atajos de teclado. Header: "Navegación, selección y reproducción"
- [x] 1.6 Crear `docs/guias-docente/sesion-03.md` — Actividad: reto cronometrado de localización, ficha de atajos
- [x] 1.7 Verificar con `mkdocs build --strict` — sin errores
- **Dependencias**: Batch 0
- **Est. líneas**: ~660

---

## Batch 2: Sesiones 4, 5 — U2: Ingreso y edición de notas I

- [ ] 2.1 Crear `docs/unidades/U-2-ingreso-edicion-notas/sesion-04/index.md` — Handbook: Basics / Note input, Notation / Accidentals, Ties. Figuras: teclas de duración, paleta de alteraciones. Header: "Ingreso de notas con teclado y ratón"
- [ ] 2.2 Crear `docs/guias-docente/sesion-04.md` — Actividad: transcripción de melodía 16 compases. Dificultades: confusión entre puntillo y ligadura
- [ ] 2.3 Crear `docs/unidades/U-2-ingreso-edicion-notas/sesion-05/index.md` — Handbook: Basics / Copy and paste, Editing notes and rests, Selection modes. Figuras: selección por rango, diálogo de filtros. Header: "Edición de alturas, duraciones y copia"
- [ ] 2.4 Crear `docs/guias-docente/sesion-05.md` — Actividad: detección de errores por parejas
- [ ] 2.5 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 1
- **Est. líneas**: ~440

---

## Batch 3: Sesiones 6, 7, 8 — U2: Compases, métrica y valores irregulares

- [ ] 3.1 Crear `docs/unidades/U-2-ingreso-edicion-notas/sesion-06/index.md` — Handbook: Basics / Measure operations, Notation / Bar lines. Figuras: diálogo de operaciones de compás. Header: "Operaciones de compás y anacrusa"
- [ ] 3.2 Crear `docs/guias-docente/sesion-06.md` — Actividad: construir fragmento con anacrusa, inserción y barras
- [ ] 3.3 Crear `docs/unidades/U-2-ingreso-edicion-notas/sesion-07/index.md` — Handbook: Notation / Time signatures, Clefs, Key signatures, Transposition; Basics / Concert pitch. Figuras: paleta de compases, diálogo de transposición. Header: "Compases, claves, armaduras y transposición"
- [ ] 3.4 Crear `docs/guias-docente/sesion-07.md` — Actividad: ejercicio con instrumentos transpositores. Dificultades: confusión entre afinación escrita y de concierto
- [ ] 3.5 Crear `docs/unidades/U-2-ingreso-edicion-notas/sesion-08/index.md` — Handbook: Notation / Tuplets, Beams, Grace notes. Figuras: diálogo de tresillo, paleta de barras. Header: "Valores irregulares, agrupación y notas de adorno"
- [ ] 3.6 Crear `docs/guias-docente/sesion-08.md` — Actividad: hoja de ejercicios rítmicos con tresillos y valores irregulares
- [ ] 3.7 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 2
- **Est. líneas**: ~660

---

## Batch 4: Sesiones 9, 10 — U3: Articulación y expresión I

- [ ] 4.1 Crear `docs/unidades/U-3-articulacion-expresion/sesion-09/index.md` — Handbook: Notation / Articulations and ornaments. Figuras: paleta de articulaciones, inspector de propiedades. Header: "Articulaciones y ornamentos"
- [ ] 4.2 Crear `docs/guias-docente/sesion-09.md` — Actividad: transcripción con acentos, staccato, fermata, trinos. Rúbrica: ubicación, coherencia, reproducción
- [ ] 4.3 Crear `docs/unidades/U-3-articulacion-expresion/sesion-10/index.md` — Handbook: Sound and Playback / Dynamics, Tempo; Text / Staff and system text. Figuras: paleta de dinámicas, diálogo de tempo. Header: "Dinámicas, tempo y texto de expresión"
- [ ] 4.4 Crear `docs/guias-docente/sesion-10.md` — Actividad: partitura con dinámicas, reguladores, cambios de tempo. Dificultades: superposición de indicaciones
- [ ] 4.5 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 3
- **Est. líneas**: ~440

---

## Batch 5: Sesiones 11, 12 — U3: Líneas y voces

- [ ] 5.1 Crear `docs/unidades/U-3-articulacion-expresion/sesion-11/index.md` — Handbook: Notation / Slurs, Arpeggios and glissandi, Lines, Octave lines. Figuras: paleta de líneas, editor de ligaduras. Header: "Líneas de notación: ligaduras, glissandi, 8va, pedal"
- [ ] 5.2 Crear `docs/guias-docente/sesion-11.md` — Actividad: partitura comentada con 5 tipos de líneas. Dificultades: diferencia entre ligadura de fraseo y prolongación
- [ ] 5.3 Crear `docs/unidades/U-3-articulacion-expresion/sesion-12/index.md` — Handbook: Basics / Voices. Figuras: selector de voces, notación por colores. Header: "Voces independientes en un pentagrama"
- [ ] 5.4 Crear `docs/guias-docente/sesion-12.md` — Actividad: fragmento polifónico a dos voces. Dificultades: colisiones, silencios innecesarios
- [ ] 5.5 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 4
- **Est. líneas**: ~480

---

## Batch 6: Sesiones 13, 14 — U4: Repeticiones y texto

- [ ] 6.1 Crear `docs/unidades/U-4-estructura-repeticiones/sesion-13/index.md` — Handbook: Notation / Repeats and jumps, Volta; Text / Rehearsal marks. Figuras: paleta de repeticiones, mapa de ruta. Header: "Signos de repetición, casillas y saltos"
- [ ] 6.2 Crear `docs/guias-docente/sesion-13.md` — Actividad: pieza breve con D.S. al Coda, casillas, marcas de ensayo
- [ ] 6.3 Crear `docs/unidades/U-4-estructura-repeticiones/sesion-14/index.md` — Handbook: Text / Text basics, Lyrics, Staff and system text, Frame text. Figuras: editor de letra, panel de estilos de texto. Header: "Texto: letra, estrofas y datos de partitura"
- [ ] 6.4 Crear `docs/guias-docente/sesion-14.md` — Actividad: partitura vocal con dos estrofas. Dificultades: separación silábica, melismas
- [ ] 6.5 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 5
- **Est. líneas**: ~480

---

## Batch 7: Sesiones 15, 16 — Integración interciclo + Examen interciclo

- [ ] 7.1 Crear `docs/unidades/U-4-estructura-repeticiones/sesion-15/index.md` — Revisión U1-U4. ≤2 bloques teoría, ≥60% ejercicios/Classroom. Figuras: síntesis de atajos clave. Header: "Integración del primer interciclo"
- [ ] 7.2 Crear `docs/guias-docente/sesion-15.md` — Esquema: Práctica ≥80 min, Desarrollo ≤20 min. Simulación de examen
- [ ] 7.3 Crear/modificar `docs/examen-interciclo.md` — Evaluación práctica 2h. Estructura: configuración (3%), alturas/ritmo (8%), expresión (6%), presentación (3%). Instrucciones de entrega Classroom
- [ ] 7.4 Actualizar `docs/unidades/U-4-estructura-repeticiones/sesion-16/index.md` — Contenido breve con referencia cruzada a examen-interciclo.md
- [ ] 7.5 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 6
- **Est. líneas**: ~320

---

## Batch 8: Sesiones 17, 18, 19 — U5: Notaciones especializadas I

- [ ] 8.1 Crear `docs/unidades/U-5-notaciones-especializadas/sesion-17/index.md` — Handbook: Text / Chord symbols; Notation / Fretboard diagrams. Figuras: editor de cifrado, paleta de diagramas. Header: "Símbolos de acordes y diagramas de guitarra"
- [ ] 8.2 Crear `docs/guias-docente/sesion-17.md` — Actividad: hoja guía para ensamble popular con melodía, cifrado y marcas
- [ ] 8.3 Crear `docs/unidades/U-5-notaciones-especializadas/sesion-18/index.md` — Handbook: Notation / Drum notation. Figuras: paleta de batería, mapa de percusión. Header: "Notación para instrumentos de percusión"
- [ ] 8.4 Crear `docs/guias-docente/sesion-18.md` — Actividad: partitura de batería 16 compases con variaciones y fill. Dificultades: asignación de alturas MIDI
- [ ] 8.5 Crear `docs/unidades/U-5-notaciones-especializadas/sesion-19/index.md` — Handbook: Advanced topics / Cross-staff notation. Figuras: editor de pentagrama cruzado, configuración de llaves. Header: "Escritura para piano y pentagrama cruzado"
- [ ] 8.6 Crear `docs/guias-docente/sesion-19.md` — Actividad: página de piano con notación polifónica y pentagrama cruzado
- [ ] 8.7 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 7
- **Est. líneas**: ~720

---

## Batch 9: Sesiones 20, 21 — U5: Guitarra e instrumentos transpositores

- [ ] 9.1 Crear `docs/unidades/U-5-notaciones-especializadas/sesion-20/index.md` — Handbook: Notation / Fretboard diagrams; Advanced topics / Tablature. Figuras: pentagrama + tablatura vinculados, editor de cuerda/traste. Header: "Notación para guitarra y tablatura"
- [ ] 9.2 Crear `docs/guias-docente/sesion-20.md` — Actividad: fragmento con notación estándar, tablatura y signos técnicos. Dificultades: digitación vs altura
- [ ] 9.3 Crear `docs/unidades/U-5-notaciones-especializadas/sesion-21/index.md` — Handbook: Basics / Concert pitch; Notation / Transposition. Figuras: botón de afinación de concierto, diálogo de cambio de instrumento. Header: "Instrumentos transpositores en ensambles"
- [ ] 9.4 Crear `docs/guias-docente/sesion-21.md` — Actividad: score breve en afinación escrita + exportación en concierto. Dificultades: verificación de tesitura
- [ ] 9.5 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 8
- **Est. líneas**: ~480

---

## Batch 10: Sesiones 22, 23, 24 — U6: MIDI e importación

- [ ] 10.1 Crear `docs/unidades/U-6-midi-importacion/sesion-22/index.md` — Handbook: Basics / Note input (MIDI keyboard section); Preferences. Figuras: configuración MIDI, indicador de entrada. Header: "Fundamentos MIDI e ingreso con teclado MIDI"
- [ ] 10.2 Crear `docs/guias-docente/sesion-22.md` — Actividad: dos versiones del mismo fragmento (paso a paso vs MIDI). Dificultades: latencia, cuantización
- [ ] 10.3 Crear `docs/unidades/U-6-midi-importacion/sesion-23/index.md` — Handbook: Advanced topics / MIDI import. Figuras: diálogo de importación MIDI, opciones de cuantización. Header: "Importación de archivos MIDI"
- [ ] 10.4 Crear `docs/guias-docente/sesion-23.md` — Actividad: limpieza guiada de 8 compases MIDI importado
- [ ] 10.5 Crear `docs/unidades/U-6-midi-importacion/sesion-24/index.md` — Handbook: Advanced topics / File formats; Getting Started / Save/Export/Print. Figuras: diálogo de exportación MusicXML, comparación de formatos. Header: "MusicXML e intercambio con otros editores"
- [ ] 10.6 Crear `docs/guias-docente/sesion-24.md` — Actividad: tabla comparativa MSCZ vs MusicXML vs MIDI. Informe de compatibilidad
- [ ] 10.7 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 9
- **Est. líneas**: ~720

---

## Batch 11: Sesiones 25, 26, 27 — U6-U7: Reproducción y formato

- [ ] 11.1 Crear `docs/unidades/U-6-midi-importacion/sesion-25/index.md` — Handbook: Sound and Playback / Mixer, Play mode. Figuras: panel del mezclador, controles de transporte. Header: "Reproducción como herramienta de revisión"
- [ ] 11.2 Crear `docs/guias-docente/sesion-25.md` — Actividad: detección auditiva de errores, balance con mezclador, exportación de audio
- [ ] 11.3 Crear `docs/unidades/U-7-edicion-partes-publicacion/sesion-26/index.md` — Handbook: Formatting / Layout and formatting, Page settings, Breaks and spacers. Figuras: diálogo de formato de página, panel de saltos. Header: "Diseño y formato de página"
- [ ] 11.4 Crear `docs/guias-docente/sesion-26.md` — Actividad: partitura antes/después de corrección de formato. Dificultades: saturación de sistemas
- [ ] 11.5 Crear `docs/unidades/U-7-edicion-partes-publicacion/sesion-27/index.md` — Handbook: Basics / Inspector and object properties; Advanced topics / Templates and styles. Figuras: panel de inspector, diálogo de estilos. Header: "Estilos y propiedades de elementos"
- [ ] 11.6 Crear `docs/guias-docente/sesion-27.md` — Actividad: corrección editorial con capturas antes/después. Dificultades: ajuste local vs global
- [ ] 11.7 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 10
- **Est. líneas**: ~720

---

## Batch 12: Sesiones 28, 29, 30, 31 + Examen Final (S32) — U7: Partes, exportación, QC, integración

- [ ] 12.1 Crear `docs/unidades/U-7-edicion-partes-publicacion/sesion-28/index.md` — Handbook: Advanced topics / Parts. Figuras: diálogo de partes, vista de score vs particella. Header: "Creación y gestión de particellas"
- [ ] 12.2 Crear `docs/guias-docente/sesion-28.md` — Actividad: score + 3 particellas exportadas individualmente. Dificultades: compases de espera, giros de página
- [ ] 12.3 Crear `docs/unidades/U-7-edicion-partes-publicacion/sesion-29/index.md` — Handbook: Getting Started / Save/Export/Print. Figuras: diálogo de exportación, formatos disponibles. Header: "Exportación e impresión profesional"
- [ ] 12.4 Crear `docs/guias-docente/sesion-29.md` — Actividad: paquete de publicación con MSCZ + PDF + PNG + MusicXML + MIDI + audio
- [ ] 12.5 Crear `docs/unidades/U-7-edicion-partes-publicacion/sesion-30/index.md` — Revisión U1-U7. Sin nuevas secciones del Handbook. Header: "Control de calidad de una partitura digital"
- [ ] 12.6 Crear `docs/guias-docente/sesion-30.md` — Actividad: auditoría entre pares con lista de cotejo general. Rúbrica: 4 criterios (musical, visual, estructural, entrega)
- [ ] 12.7 Crear `docs/unidades/U-7-edicion-partes-publicacion/sesion-31/index.md` — Integración final. ≤2 bloques teoría, ≥70% ejercicios. Header: "Integración final del flujo de trabajo en MuseScore"
- [ ] 12.8 Crear `docs/guias-docente/sesion-31.md` — Esquema: Práctica ≥90 min, Desarrollo ≤15 min. Caso integrador con ensamble mixto
- [ ] 12.9 Crear/modificar `docs/examen-final.md` — Evaluación práctica 2h. Estructura: configuración y exactitud (12%), herramientas avanzadas (7%), score/particellas (7%), entrega (4%). Instrucciones de entrega Classroom
- [ ] 12.10 Verificar con `mkdocs build --strict`
- **Dependencias**: Batch 11
- **Est. líneas**: ~1,010

---

## Batch 13: Verificación post-aplicación

- [ ] 13.1 Ejecutar `mkdocs build --strict` desde `/tmp/tecnomusical` — debe ser clean (0 errores, 0 warnings)
- [ ] 13.2 Verificar checklist de plantilla por sesión: glosario con anchors, ≥2 bloques teoría (`???+ note`), ≥1 Handbook figura/GIF reference, footer con atribución
- [ ] 13.3 Verificar guías docentes: header, objetivo, esquema (4 momentos), actividad Classroom, rúbrica (≥2 criterios, 3 niveles), preguntas apertura/cierre (≥2 cada una), dificultades (≥2), recursos (≥2)
- [ ] 13.4 Revisar links internos — todos los anchors de glosario deben resolver dentro de cada página
- [ ] 13.5 Verificar que ninguna página contiene MathJax (`\(`, `\[`, `\boxed{}`)
- [ ] 13.6 Inspección visual: colapsables funcionan en tema claro y oscuro (spot-check 3 sesiones)
- [ ] 13.7 Reportar: número de archivos creados/modificados, build status, checklist compliance %
- **Dependencias**: Batch 12
- **Criterio**: `mkdocs build --strict` exit 0; 31 sesiones + 32 guías + 2 exámenes existen y pasan checklist; zero MathJax rendering
