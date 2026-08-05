# Design: Preparar Sesiones Tecnomusical

## Architecture Overview

This change is content-only for a Material for MkDocs documentation site.
No code, no database, no API. The design centers on the **session page template**
and the **content pipeline** from the MuseScore Handbook to MkDocs Markdown.

## Session Page Template

Each `docs/unidades/U-{n}-*/sesion-{NN}/index.md` follows this structure:

```markdown
# Sesión N: Título

📚 Handbook → [sección] | Herramientas: MuseScore Studio 4, [otros]

## Glosario

??? info "Glosario de términos"
    | Término | Definición |
    |---------|------------|
    | <a id="ancla"></a> **término** | definición |

## Teoría

???+ note "Título del bloque 1"
    Contenido del Handbook...
    > Insertar [captura/Fig. X-Y] del Handbook: descripción breve

???+ note "Título del bloque 2"
    ...

## Actividad en Classroom

1. Paso 1
2. Paso 2
...

### Entregables
- Archivo .mscz
- PDF exportado

### Autoevaluación
| Criterio | ✅ | ⚠️ | ❌ |
|----------|----|----|-----|
| ... | | | |

---

*Basado en: MuseScore 3 Handbook — [sección] | https://musescore.org/en/handbook/3*
```

### Key Decisions

1. **No MathJax**: Tecnomusical teaches GUI operations, not formulas. The `extra_javascript` and `markdown_extensions.mathjax` entries in mkdocs.yml remain but are unused by Tecnomusical pages. No harm in keeping them.

2. **Collapsible glossary vs. inline**: Glossary uses MkDocs Material `??? info` admonitions (collapsed by default). This reduces vertical scroll while keeping terminology discoverable.

3. **Collapsible theory blocks**: Theory uses `???+ note` admonitions (expanded by default, individually collapsible). Each block covers one Handbook subsection.

4. **Figure/GIF references as blockquotes**: `> Insertar...` convention avoids broken images. The instructor inserts actual screenshots/GIFs post-generation. References include Handbook section identifiers for easy retrieval.

5. **No iframe embeds**: Unlike Acústica (p5.js simulations), Tecnomusical pages do not embed interactive assets. All interactivity happens inside MuseScore Studio.

## Guía Docente Template

```
docs/guias-docente/sesion-NN.md
```

Structure:

```markdown
# Guía Docente — Sesión N: Título

**Duración estimada**: 1 sesión presencial (≈ 2 horas)
**Herramientas**: MuseScore Studio 4, proyector, Google Classroom
**Referencia**: MuseScore 3 Handbook — [sección]

## Objetivo de la sesión
Que el estudiante [verbo] [competencia].

## Esquema de la clase
| Momento | Duración | Actividad |
|---------|----------|-----------|
| Apertura | 10 min | ... |
| Desarrollo | 25 min | ... |
| Práctica | 70 min | ... |
| Cierre | 15 min | ... |

## Actividad en Classroom
### Tarea: [título]
...

### Rúbrica
...

## Preguntas para discusión
### Apertura
- ...
### Cierre
- ...

## Posibles dificultades
| Problema | Solución |
|----------|----------|
| ... | ... |

## Recursos adicionales
- [Handbook section link]
- [Video tutorial reference]
```

## Content Pipeline

```
MuseScore 3 Handbook (online)
    │
    ▼
Session plan (plan_32_sesiones_*.txt)
    │  → Maps session → Handbook section
    ▼
Agent drafts session page (index.md) + guía docente (sesion-NN.md)
    │
    ▼
mkdocs build --strict → site/
```

The agent is the content writer, not a scraper. It reads the Handbook, synthesizes
key concepts, and produces Spanish-language educational content for each session.
The agent does NOT copy-paste Handbook text verbatim — it adapts for a university course context.

## Delivery Architecture

```
Batch → PR (each batch = 1 PR targeting main)
  ├── Session pages (2–4 per batch)
  ├── Guías docentes (matched 1:1)
  └── Verification: mkdocs build --strict
```

12 batches, each producing one PR. Per-batch verification ensures regressions
are isolated. Rollback is `git revert` on the offending PR — no cross-batch
coupling.

## File Count

| Type | Count | Path pattern |
|------|-------|-------------|
| Session pages (content) | 31 | `docs/unidades/U-*/sesion-{NN}/index.md` |
| Exam pages | 2 | `docs/examen-*.md` |
| Guías docentes | 32 | `docs/guias-docente/sesion-{NN}.md` |
| **Total files** | **65** | |
