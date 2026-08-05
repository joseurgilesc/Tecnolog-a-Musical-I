# guia-docente-tecnomusical Specification

## Purpose

Spec for teacher guides (`docs/guias-docente/sesion-NN.md`). Each guide MUST provide
a class plan with timing, Classroom activity, rubric, discussion prompts, and
anticipated difficulties. Replicates the Acústica guía docente template.

## Requirements

### Requirement: Guide Header
The guide MUST open with `# Guía Docente — Sesión N: Título` and a metadata block:
Duración estimada, Herramientas, and Referencia (Handbook section).

#### Scenario: Standard guide header
- GIVEN a guide for session 4 "Ingreso de notas"
- WHEN rendered
- THEN H1 reads "# Guía Docente — Sesión 4: Ingreso de notas"
- AND metadata includes "Duración estimada: 1 sesión presencial (≈ 2 horas)"
- AND "Referencia: MuseScore 3 Handbook — Basics / Note input"

### Requirement: Session Objective
A single-sentence objective MUST follow the header, describing what the student
will achieve by session end.

#### Scenario: Objective is observable and software-specific
- GIVEN session 4 covers note input
- WHEN the objective is written
- THEN it follows the form "Que el estudiante [verbo observable] [competencia MuseScore]"
- AND it references a measurable outcome (e.g., "transcriba una melodía de 16 compases usando el teclado del computador")

### Requirement: Class Schema with Timing
The guide MUST include an "Esquema de la clase" table with four moments:
Apertura, Desarrollo, Práctica, Cierre. Each row MUST have duration and activity.
Timing follows: Apertura 10 min, Desarrollo 25 min, Práctica 70 min, Cierre 15 min.

#### Scenario: Standard class schema
- GIVEN a hands-on MuseScore session
- WHEN the schema renders
- THEN Apertura ≤15 min, Desarrollo ≤30 min, Práctica ≥60 min, Cierre ≤15 min
- AND total duration is 120 min (2 hours)

#### Scenario: Integration session extends practice
- GIVEN session 31 (integración final)
- WHEN the schema renders
- THEN Práctica ≥80 min and Desarrollo ≤20 min
- AND Apertura reviews previous concepts in ≤10 min

### Requirement: Classroom Activity
The guide MUST include a copy-ready Classroom activity block with: title,
step-by-step instructions, deliverable list, and self-assessment checklist.
Tagged as "Tarea" (Google Classroom Task).

#### Scenario: Activity with step-by-step instructions
- GIVEN session 4 is a transcription exercise
- WHEN the activity block renders
- THEN instructions are numbered sequentially
- AND deliverables include ".mscz, PDF, and screenshot of input mode"
- AND a checklist table with ≥3 criteria follows

#### Scenario: Exam session guide (S16, S32)
- GIVEN an exam session guide
- WHEN the activity block renders
- THEN it describes evaluation structure, time limits, and submission requirements
- AND includes rúbrica de evaluación with weighted criteria matching the evaluation plan

### Requirement: Formative Rubric
The activity MUST be accompanied by a 3-level rubric table
(✅ Logrado | ⚠️ En proceso | ❌ No logrado) with at least 2 criteria rows.

#### Scenario: Rubric with software-specific criteria
- GIVEN a Classroom activity for note input
- WHEN the rubric renders
- THEN it has ≥2 criteria (e.g., "Exactitud de alturas y ritmos", "Exportación correcta a PDF")
- AND each criterion has distinct descriptors for all 3 levels

#### Scenario: Session 1 rubric is minimal
- GIVEN session 1 (introduction, diagnostic focus)
- WHEN the rubric renders
- THEN it has 2 criteria max (instalación/configuración + reflexión)
- AND descriptors are qualitative rather than quantitative

### Requirement: Discussion Questions
The guide MUST include ≥2 opening questions (Apertura) and ≥2 closing questions
(Cierre). Closing questions MUST connect session concepts to musical practice.

#### Scenario: Closing questions bridge to real-world use
- GIVEN session 4 covers note input
- WHEN closing questions render
- THEN at least one connects to professional practice (e.g., "¿Para qué tipo de proyectos usarías el ingreso con ratón vs. teclado MIDI?")

#### Scenario: Opening questions surface prior knowledge
- GIVEN session 7 builds on session 6
- WHEN opening questions render
- THEN at least one question references the previous session's concept

### Requirement: Anticipated Difficulties
The guide MUST include a "Posibles dificultades" table with Problem | Solution rows,
covering ≥2 common student mistakes for the session topic.

#### Scenario: Difficulties table for UI-heavy session
- GIVEN session 12 covers voices
- WHEN the difficulties table renders
- THEN it includes a row for "Confusión entre voz 1 y voz 2 durante la edición"
- AND the solution proposes color-coding and voice isolation strategies

### Requirement: Additional Resources
The guide MUST end with a "Recursos adicionales" section listing ≥2 external
references: Handbook links, video tutorials, or official MuseScore resources.
