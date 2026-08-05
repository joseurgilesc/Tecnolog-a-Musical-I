# sesion-tecnomusical-content Specification

## Purpose

Spec for student-facing MkDocs session pages (`docs/unidades/U-{n}-*/sesion-{NN}/index.md`).
Each page MUST present curated MuseScore Handbook content via collapsible glossary, theory sections,
and figure/GIF references. Replicates the Acústica template without MathJax (MuseScore is GUI-driven).

## Requirements

### Requirement: Session Header
The page MUST open with `# Sesión N: Título` and a metadata block listing handbook reference
(📚) and software/tools (Herramientas).

#### Scenario: Standard session renders header correctly
- GIVEN a session page with number 4 and title "Ingreso de notas"
- WHEN the page is built via mkdocs
- THEN the H1 reads "# Sesión 4: Ingreso de notas"
- AND metadata shows "📚 Handbook → Basics / Note input | Herramientas: MuseScore Studio 4, teclado MIDI"

### Requirement: Collapsible Glossary
The page MUST include a `??? info` glossary table with musical and software terminology.
Each entry MUST have an HTML anchor (`<a id="...">`) for cross-reference.
Term and definition columns are mandatory.

#### Scenario: Standard glossary with software and musical terms
- GIVEN a session covering note input
- WHEN the glossary section is rendered
- THEN entries for "pentagrama", "compás", "figura", "silencio", "alteración", "modo de entrada" are present with anchors
- AND each anchor uses a stable id (e.g., `id="modo-entrada"`)

#### Scenario: Session 1 glossary covers basic UI terminology
- GIVEN session 1 (introduction, no deep notation)
- WHEN the glossary is rendered
- THEN it contains terms: "MSCZ", "MusicXML", "MIDI", "paleta", "panel de propiedades", "mezclador" — max 10 entries
- AND no specialized notation symbols appear

### Requirement: Collapsible Theory Sections
Theory content MUST be organized as `???+ note` collapsible blocks, one per topic.
Content MUST be sourced from the MuseScore Handbook section mapped in the proposal.

#### Scenario: Multi-topic session renders distinct collapsible sections
- GIVEN session 4 mapped to Handbook "Basics / Note input"
- WHEN the page is rendered
- THEN at least 2 `???+ note` blocks appear (e.g., "Ingreso con teclado de computador", "Duración y silencios")
- AND each section is independently collapsible

#### Scenario: Integration session emphasizes activities over new theory
- GIVEN session 15 (integration U1-U4)
- WHEN the page is rendered
- THEN theory sections are ≤2 blocks of review/synthesis
- AND practical exercises comprise ≥60% of the page

### Requirement: Handbook Figure and GIF References
Each theory section that covers a GUI operation MUST include a blockquote referencing
the relevant Handbook figure or screenshot.
Format: `> Insertar Fig. X-Y del Handbook: [descripción de la operación mostrada]`.
For UI workflows, screenshots/GIFs MUST reference the specific Handbook page section.

#### Scenario: Figure reference present for GUI operation
- GIVEN session 4 covers note input via computer keyboard
- WHEN the theory section renders
- THEN `> Insertar captura de la sección "Note input → Basic note entry" del Handbook: teclas de duración resaltadas` appears

#### Scenario: Session without applicable figure
- GIVEN a theory section on a conceptual topic without a Handbook screenshot
- WHEN the section renders
- THEN no figure reference blockquote is emitted
- AND the section does not fabricate a reference

### Requirement: Classroom Activity Instructions
The page MUST include a `## Actividad en Classroom` section with numbered steps,
expected deliverables, and a self-assessment checklist.

#### Scenario: Activity with clear deliverables
- GIVEN session 4 is a transcription exercise
- WHEN the activity section renders
- THEN steps are numbered (1..N)
- AND expected deliverables include ".mscz and PDF export"
- AND a checklist table (✅ | ⚠️ | ❌) with ≥3 criteria is present

### Requirement: No MathJax
The page MUST NOT use MathJax or display formulas. All notation is described
via GUI operations, keyboard shortcuts, and terminology.

#### Scenario: No formula rendering
- GIVEN any Tecnomusical session page
- WHEN the page is built via mkdocs
- THEN zero `\(`, `\[`, or `\boxed{}` MathJax statements appear
- AND musical concepts are explained via prose and UI descriptions

### Requirement: Session Footer
The page MUST end with a `---` separator followed by a handbook attribution line:
`*Basado en: MuseScore 3 Handbook — [sección]*` and a link to the official manual.

#### Scenario: Footer with handbook attribution
- GIVEN session 4 content
- WHEN the page footer renders
- THEN `*Basado en: MuseScore 3 Handbook — Basics / Note input*` appears
- AND the link `https://musescore.org/en/handbook/3` is present
