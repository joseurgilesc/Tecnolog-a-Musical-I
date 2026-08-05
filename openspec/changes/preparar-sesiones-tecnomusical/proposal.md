# Proposal: Preparar Sesiones Tecnomusical

## Intent

Fill 31 MkDocs session pages (S1–S15, S17–S31) and 32 guías docentes with curated content from the MuseScore 3 Handbook, replacing `<!-- Contenido pendiente -->` placeholders. The format replicates Acústica: collapsible glossary, collapsible theory sections, handbook figure/GIF references, and standalone guías docentes. Exam pages (S16, S32) are also filled with evaluation instructions.

## Scope

### In Scope

- 31 student-facing `index.md` files following the Acústica session template:
  - `??? info` glossary with software/musical terminology (no formulas — no MathJax)
  - `???+ note` theory sections sourced from MuseScore 3 Handbook
  - Handbook figure references (`> Insertar Fig. X-Y del Handbook: descripción`)
  - GIF/screenshot references for UI operations
  - Classroom activity instructions and checklist
- 32 guías docentes (`docs/guias-docente/sesion-NN.md`): class schema, rubric, discussion questions, anticipated difficulties
- 2 exam pages: `docs/examen-interciclo.md` (S16) and `docs/examen-final.md` (S32) with full evaluation specs
- Handbook session mapping validated against the 32-session plan

### Out of Scope

- Creating new screenshots or GIFs (references only)
- Modifying `mkdocs.yml` nav (already complete with 7 units + exams)
- New interactive assets (no p5.js, Tone.js — not applicable to MuseScore)
- Modifying `docs/index.md`, `docs/objetivos.md`, `docs/logros.md` (already complete)
- Unit `index.md` pages (already complete with session links)

## Capabilities

### New Capabilities

- `sesion-tecnomusical-content`: full student-facing session page with MuseScore Handbook-sourced collapsible glossary, theory sections, and GUI operation references
- `guia-docente-tecnomusical`: teacher guide with class schema, rubric, discussion prompts, and anticipated difficulties

### Modified Capabilities

None — this is new content, not spec-level changes.

## Approach

1. **Agent maps** every session to MuseScore Handbook sections (see mapping below)
2. **Agent drafts** each session iteratively — student page then guía docente — in chronological order
3. Each session embeds collapsible glossary with musical/software terms (no MathJax — MuseScore is GUI-driven)
4. Handbook figures/GIFs are referenced by section and description — no new graphics generated
5. Guías docentes follow the same structure as Acústica: header, objective, class schema, Classroom activity, rubric, discussion questions, difficulties, resources

### MuseScore 3 Handbook Mapping

| Session | Topic | Handbook Section(s) |
|---------|-------|---------------------|
| S1 | Introducción, instalación, formatos | Getting Started → Download and Installation, Create new score, Language; Basics → Viewing and navigation |
| S2 | Creación de partitura, instrumentos, plantillas | Basics → Create new score, Instruments, Score properties; Notation → Key signatures, Time signatures |
| S3 | Navegación, selección, reproducción básica | Basics → Viewing and navigation, Selection modes, Undo and redo; Sound and Playback → Play mode |
| S4 | Ingreso de notas: teclado y ratón | Basics → Note input; Notation → Accidentals, Ties |
| S5 | Edición de alturas, copia/pega, filtros | Basics → Copy and paste, Editing notes and rests, Selection modes |
| S6 | Operaciones de compás, anacrusa, barras | Basics → Measure operations; Notation → Bar lines |
| S7 | Compases, claves, armaduras, transposición | Notation → Time signatures, Clefs, Key signatures, Transposition; Basics → Concert pitch |
| S8 | Valores irregulares, agrupación, notas de adorno | Notation → Tuplets, Beams, Grace notes |
| S9 | Articulaciones y ornamentos | Notation → Articulations and ornaments |
| S10 | Dinámicas, tempo, texto de expresión | Sound and Playback → Dynamics, Tempo; Text → Staff and system text |
| S11 | Líneas: ligaduras, glissandi, 8va, pedal | Notation → Slurs, Arpeggios and glissandi, Lines, Octave lines |
| S12 | Voces independientes | Basics → Voices |
| S13 | Repeticiones, casillas, D.C., D.S., Coda | Notation → Repeats and jumps, Volta; Text → Rehearsal marks |
| S14 | Texto, letra, estrofas | Text → Text basics, Lyrics, Staff and system text, Frame text |
| S15 | Integración primer interciclo | Review — no new handbook sections |
| S17 | Símbolos de acordes, diagramas de guitarra | Text → Chord symbols; Notation → Fretboard diagrams |
| S18 | Notación para percusión | Notation → Drum notation |
| S19 | Escritura para piano, pentagrama cruzado | Advanced topics → Cross-staff notation |
| S20 | Guitarra, tablatura | Notation → Fretboard diagrams; Advanced topics → Tablature |
| S21 | Instrumentos transpositores en ensambles | Basics → Concert pitch; Notation → Transposition |
| S22 | Fundamentos MIDI, teclado MIDI | Basics → Note input (MIDI keyboard); Preferences |
| S23 | Importación de archivos MIDI | Advanced topics → MIDI import |
| S24 | MusicXML, intercambio con otros editores | Advanced topics → File formats; Getting Started → Save/Export/Print |
| S25 | Reproducción, mezclador, balance | Sound and Playback → Mixer, Play mode |
| S26 | Diseño y formato de página | Formatting → Layout and formatting, Page settings, Breaks and spacers |
| S27 | Estilos y propiedades de elementos | Basics → Inspector and object properties; Advanced topics → Templates and styles |
| S28 | Creación y gestión de particellas | Advanced topics → Parts |
| S29 | Exportación e impresión | Getting Started → Save/Export/Print |
| S30 | Control de calidad de partitura digital | Review — no new handbook sections |
| S31 | Integración final del flujo de trabajo | Review — no new handbook sections |

## Affected Areas

| Area | Impact | Description |
|------|--------|-------------|
| `docs/unidades/U-{1..7}-*/sesion-{NN}/index.md` | Modified (32 files) | Replace placeholders with Handbook content |
| `docs/guias-docente/sesion-{NN}.md` | New (32 files) | Create teacher guides |
| `docs/examen-interciclo.md` | Modified | Fill evaluation instructions (S16) |
| `docs/examen-final.md` | Modified | Fill evaluation instructions (S32) |
| `mkdocs.yml` | Unchanged | Nav already complete |

## Risks

| Risk | Likelihood | Mitigation |
|------|------------|------------|
| Handbook version mismatch (MS3 vs MS4 UI differences) | Med | Cross-reference MS4 official handbook before each batch; note version warnings in content |
| Content volume (~7,000+ lines, ~12 PRs exceeding 400-line budget) | High | User accepted per-batch PRs; use auto-chain with size exception |
| Inconsistency between student pages and guías docentes | Low | Draft each pair together (student page → guía) before moving to next session |
| Figure/GIF references point to missing or relocated handbook assets | Med | Reference by section name, not URL; provide stable Handbook § references |

## Rollback Plan

- Content-only change. Revert via `git revert` on the delivery branch.
- No database migrations, no config changes, no deployment impact beyond `mkdocs build`.

## Dependencies

- MuseScore 3 Handbook: https://musescore.org/en/handbook/3
- Plan de sesiones: `/Users/jose/Documents/PreparaciónClases/Tecnología Musical I/plan_32_sesiones_tecnologia_musical_I_musescore.txt`
- MkDocs site skeleton already exists at `/tmp/tecnomusical`

## Success Criteria

- [ ] All 31 student pages render correctly via `mkdocs build --strict`
- [ ] All 32 guías docentes exist in `docs/guias-docente/`
- [ ] Every session includes: glossary, ≥2 theory sections, ≥1 Handbook figure/GIF reference
- [ ] Exam pages (S16, S32) include full evaluation structure
- [ ] No new binaries, images, or interactive assets created (reference-only)
- [ ] Handbook section references are accurate and verifiable
