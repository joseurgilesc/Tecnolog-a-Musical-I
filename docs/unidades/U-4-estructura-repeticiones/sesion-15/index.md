# Sesión 15: Integración del primer interciclo

📚 Handbook → Revisión: Getting Started, Basics, Notation, Sound and Playback, Text | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos (repaso U1–U4)"
    Consultá esta tabla cuando encuentres un término que no recuerdes.

    | Término | Definición |
    |---|---|
    | <a id="partitura"></a> **Partitura (score)** | Archivo `.mscz` que contiene toda la música: pentagramas, notas, indicaciones, diseño. Es el documento principal de MuseScore. Se crea desde el asistente de nueva partitura seleccionando plantilla, instrumentos, armadura, compás y tempo. |
    | <a id="nota"></a> **Nota** | Unidad mínima de sonido en una partitura. Tiene tres propiedades: altura (qué tecla/posición en el pentagrama), duración (negra, corchea, etc.) y articulación (cómo se ataca). Se ingresa con el modo de ingreso de notas (`N`), usando letras del teclado (A–G) o el mouse sobre el pentagrama. |
    | <a id="compas"></a> **Compás (measure)** | División del tiempo musical en unidades regulares definidas por la indicación de compás (ej. 4/4, 3/4, 6/8). Las operaciones de compás incluyen insertar, eliminar, unir, dividir y ajustar la duración real (*Measure Properties*). |
    | <a id="armadura"></a> **Armadura de clave (key signature)** | Conjunto de sostenidos o bemoles al inicio del pentagrama que define la tonalidad. Determina qué notas son alteradas por defecto en toda la pieza. Se cambia arrastrando una nueva armadura desde la paleta. |
    | <a id="clave"></a> **Clave (clef)** | Símbolo al inicio del pentagrama que asigna nombres a las líneas y espacios (Sol, Fa, Do). Cambiar la clave altera la posición visual de las notas sin cambiar su sonido. |
    | <a id="valor-irregular"></a> **Valor irregular (tuplet)** | Grupo de notas que ocupa un tiempo distinto al que le correspondería por su figura. El más común es el tresillo (3 corcheas en tiempo de 2). En MuseScore se crea con **Añadir → Tresillos → Otro**. |
    | <a id="articulacion"></a> **Articulación (articulation)** | Indicación sobre una nota que modifica su ataque o duración: acento (>), staccato (.), tenuto (–), fermata (𝄐), trino (*tr*), mordente. Se arrastran desde la paleta **Articulaciones**. |
    | <a id="dinamica"></a> **Dinámica (dynamics)** | Indicación de intensidad: *pp, p, mp, mf, f, ff*, reguladores de crescendo y diminuendo (`<` y `>`). En MuseScore se arrastran desde la paleta **Dinámicas** y afectan la reproducción. |
    | <a id="voz"></a> **Voz (voice)** | Capa rítmicamente independiente dentro de un mismo pentagrama. MuseScore permite hasta 4 voces por pentagrama, cada una con sus propias plicas, silencios y colores. Se activan con los botones 1–4 de la barra de herramientas. |
    | <a id="repeticion"></a> **Repetición (repeat)** | Sistema de marcas que modifican el orden de ejecución: barras de repetición, voltas (casillas 1 y 2), D.C., D.S., Coda, Fine. Se arrastran desde la paleta **Repeticiones y saltos** y afectan la reproducción. |
    | <a id="texto-expresion"></a> **Texto de expresión (staff/system text)** | Indicaciones textuales sobre la partitura. Staff Text (`Ctrl + T`) se aplica a un pentagrama; System Text (`Ctrl + Shift + T`) a todos los pentagramas. Se usan para tempo, carácter, técnicas instrumentales y marcas de ensayo. |
    | <a id="guardar-exportar"></a> **Guardar y exportar** | MuseScore guarda en formato nativo `.mscz` (editable). Exporta a PDF, PNG, MusicXML, MIDI, MP3 y otros formatos desde **Archivo → Exportar**. |

???+ note "Mapa conceptual: flujo de trabajo U1–U4"

    **De la instalación a la partitura completa en 4 unidades.**

    ```
    U1 — FUNDAMENTOS              U2 — NOTAS Y EDICIÓN          U3 — EXPRESIÓN                 U4 — ESTRUCTURA
    ┌──────────────────┐         ┌──────────────────┐         ┌──────────────────┐         ┌──────────────────┐
    │ ▪ Instalación     │         │ ▪ Ingreso de notas │        │ ▪ Articulaciones  │         │ ▪ Repeticiones    │
    │ ▪ Nueva partitura │  ────▶  │ ▪ Teclado y ratón  │ ────▶ │ ▪ Dinámicas       │ ────▶  │ ▪ Voltas y saltos │
    │ ▪ Navegación      │         │ ▪ Edición, copia   │        │ ▪ Líneas          │         │ ▪ Texto y letra   │
    │ ▪ Selección       │         │ ▪ Compases, claves │        │ ▪ Voces           │         │ ▪ Cifrado armónico│
    └──────────────────┘         └──────────────────┘         └──────────────────┘         └──────────────────┘
         "Sé abrir el                 "Sé escribir                  "Sé hacer que                 "Sé organizar la
          programa y                   las notas                    suene como                    pieza y ponerle
          crear un archivo"            correctamente"               quiero"                       nombre a todo"
    ```

    Cada unidad construye sobre la anterior. Si algo de U1 no funciona (no sabés crear una partitura), U2 se vuelve imposible. Si U2 falla (no sabés ingresar notas), no podés aplicar articulaciones en U3. Si U3 falla, en U4 estás poniendo repeticiones y letra sobre una partitura que no suena bien.

    La integración es la habilidad de USAR TODO JUNTO. No se trata de recordar cada atajo de teclado: se trata de saber qué herramienta usar en cada momento del flujo de trabajo.

???+ note "Checklist pre-examen: ¿estoy listo para el interciclo?"

    Repasá cada punto. Si algo no te sale en ≤2 minutos, repasalo antes del examen.

    ### U1 — Instalación y organización del trabajo

    | # | ¿Puedo...? | ✅/❌ |
    |---|-----------|------|
    | 1 | Abrir MuseScore Studio 4 y crear una partitura nueva seleccionando plantilla, instrumentos, armadura y compás | |
    | 2 | Navegar entre páginas con el scroll, usar los modos de visualización (Normal, Página, Continuo) y el zoom | |
    | 3 | Seleccionar compases completos (clic en espacio vacío), notas individuales (clic en cabeza), rangos (`Shift + clic`) | |
    | 4 | Guardar como `.mscz`, exportar como PDF y PNG | |
    | 5 | Usar `Ctrl + Z` (deshacer) y `Ctrl + Shift + Z` (rehacer) para corregir errores | |

    ### U2 — Ingreso y edición de notas

    | # | ¿Puedo...? | ✅/❌ |
    |---|-----------|------|
    | 6 | Ingresar notas con el teclado (letras A–G) y el mouse, cambiando duraciones (5=negra, 4=corchea, etc.) | |
    | 7 | Ingresar alteraciones (sostenido, bemol, becuadro) y ligaduras de prolongación (`T`) | |
    | 8 | Copiar uno o varios compases y pegarlos en otra sección (`Ctrl + C` / `Ctrl + V`) | |
    | 9 | Editar la altura de una nota (arrastrar con el mouse o `↑` / `↓`) y su duración (seleccionar + número) | |
    | 10 | Insertar, eliminar, unir y dividir compases desde **Añadir → Compases** o el menú contextual | |
    | 11 | Crear un compás de anacrusa (compás incompleto al inicio) desde **Propiedades del compás** | |
    | 12 | Cambiar la indicación de compás (arrastrar desde paleta) y la armadura de clave | |
    | 13 | Cambiar la clave de un pentagrama sin alterar el sonido | |
    | 14 | Crear un tresillo de corcheas u otro valor irregular desde **Añadir → Tresillos** | |
    | 15 | Activar el modo de **altura de concierto** y verificar que los instrumentos transpositores muestren las notas correctas | |

    ### U3 — Articulación, expresión y reproducción

    | # | ¿Puedo...? | ✅/❌ |
    |---|-----------|------|
    | 16 | Insertar acentos (>), staccatos (.), tenutos (–), fermatas y trinos desde la paleta **Articulaciones** | |
    | 17 | Insertar dinámicas (*pp, p, mp, mf, f, ff*), reguladores de crescendo y diminuendo desde la paleta **Dinámicas** | |
    | 18 | Insertar indicaciones de tempo y cambios de tempo con texto de sistema (`Ctrl + Shift + T`) | |
    | 19 | Insertar líneas: ligaduras de expresión (`S`), 8va/8vb, pedal de piano, glissandos/arpegios, comas de respiración | |
    | 20 | Activar, escribir y diferenciar voces 1 y 2 en un mismo pentagrama (colores, plicas, silencios) | |
    | 21 | Intercambiar el contenido de voces 1 ↔ 2 sin perder notas | |

    ### U4 — Estructura, repeticiones y texto

    | # | ¿Puedo...? | ✅/❌ |
    |---|-----------|------|
    | 22 | Insertar barras de repetición (inicio, fin, fin-inicio) y verificar que la reproducción las ejecuta correctamente | |
    | 23 | Insertar voltas (casillas 1 y 2) desde la paleta y configurar su lista de repetición en Propiedades | |
    | 24 | Insertar D.C., D.S., Segno, Coda y Fine, formando un mapa de navegación que funcione en la reproducción | |
    | 25 | Ingresar letra debajo de una melodía vocal usando `Ctrl + L`, con guiones silábicos (`-`) y melismas (`_`) | |
    | 26 | Insertar cifrado armónico sobre un pentagrama usando `Ctrl + K` (mayores, menores, séptimas, bajo alterado) | |
    | 27 | Insertar Staff Text (`Ctrl + T`) y System Text (`Ctrl + Shift + T`) y distinguir cuándo usar cada uno | |
    | 28 | Insertar marcas de ensayo (`Ctrl + M`) en puntos estructurales de la partitura | |

    **Resultado:** ___ / 28

    *Regla:* si tenés ≥22 ✅, estás listo para el examen. Si tenés entre 15 y 21, repasá las secciones marcadas ❌. Si tenés ≤14, necesitás una sesión de tutoría antes del examen.

---

## Actividad en Classroom

### Tarea: S15 — Simulacro de examen interciclo

> **Material necesario**: el docente proporcionará un archivo `simulacro_interciclo_S15.mscz` que contiene una partitura base con la melodía "Estrellita dónde estás" en Do mayor, 4/4, 8 compases, un solo pentagrama en clave de Sol, con la melodía escrita en redondas (una nota por compás) y SIN indicaciones de ningún tipo (sin dinámicas, sin articulaciones, sin repeticiones, sin texto, sin letra, sin cifrado). También recibirás el archivo `simulacro_voces_S15.mscz` con un coral a 2 voces en Fa mayor, 4/4, 8 compases, con ambas voces escritas pero SIN indicaciones. El docente entregará además las **Instrucciones oficiales del simulacro** como Tarea en Classroom que incluya: la consigna completa del caso integrador, los criterios de evaluación con puntajes, y las preguntas conceptuales y procedimentales.

Esta actividad es un **simulacro del examen interciclo**. Vas a trabajar en condiciones similares a las del examen real: tiempo limitado (90 minutos), sin ayuda externa, aplicando todo lo aprendido de U1 a U4.

**IMPORTANTE**: Leé TODAS las instrucciones antes de empezar. El simulacro tiene 4 partes, igual que el examen real. Administrá tu tiempo: no te quedes atascado en una parte.

---

### Parte 1 — Conceptual (≈15 minutos, 25%)

Respondé en un comentario de Classroom las siguientes preguntas. Cada respuesta debe ser breve (2–4 oraciones) y concreta:

1. **Flujo de trabajo**: Describí los 4 pasos que seguís para crear una partitura desde cero en MuseScore. ¿En qué orden los hacés y por qué?

2. **Voces vs. pentagramas**: ¿Cuándo usarías 2 voces en un mismo pentagrama en lugar de 2 pentagramas separados? Da un ejemplo concreto de cada caso.

3. **Repeticiones con navegación**: Explicá la diferencia entre una volta (casilla 1/2) y un D.S. al Coda. ¿En qué situación usarías cada uno?

4. **Texto en la partitura**: Diferenciá Staff Text de System Text. Da un ejemplo concreto de cada uno en una partitura de cuerdas.

5. **Armadura y transporte**: Si tenés una partitura para Clarinete en Si♭ (instrumento transpositor), ¿las notas que escribiste en el pentagrama suenan igual que las que ves? Explicá por qué y cómo verificarías que todo está correcto.

---

### Parte 2 — Procedimental (≈15 minutos, 25%)

Abrí el archivo `simulacro_interciclo_S15.mscz` y realizá las siguientes operaciones. Para cada una, anotá en tu comentario de Classroom **el atajo de teclado o la ruta de menú** que usaste:

1. Cambiar la indicación de compás de 4/4 a 3/4.
2. Agregar un sostenido a la armadura (Do mayor → Sol mayor).
3. Insertar un compás de anacrusa de 1 tiempo (negra) al inicio de la partitura.
4. Seleccionar los compases 3 al 6 y copiarlos al final de la partitura (compases 9 al 12).
5. Cambiar la clave del pentagrama de Sol a Fa en 4ª.
6. Crear un tresillo de corcheas en el compás 2.
7. Insertar una barra de repetición de inicio en el compás 1 y de fin en el compás 8.
8. Agregar dinámica *mf* al compás 1 y *f* al compás 5.

> *Nota*: No es necesario que guardes el archivo. Solo necesitás demostrar que SABÉS CÓMO hacerlo.

---

### Parte 3 — Ejercicios de aplicación (≈25 minutos, 25%)

Usando el archivo `simulacro_interciclo_S15.mscz` como base:

1. **Articulaciones**: Agregá sobre las notas de los compases 1–4:
   - Un acento en la primera nota de cada compás.
   - Un staccato en las notas de duración más corta.
   - Un trino sobre la última nota del compás 4.

2. **Dinámicas**: Insertá:
   - *mp* al inicio del compás 1.
   - Un regulador de crescendo desde el compás 3 hasta el compás 4.
   - *f* al inicio del compás 5.
   - Un regulador de diminuendo desde el compás 7 hasta el compás 8.
   - *pp* al final del compás 8.

3. **Líneas**: Insertá:
   - Una ligadura de expresión sobre los compases 1 y 2.
   - Un pedal de piano (línea Ped.) desde el compás 3 hasta el compás 6, con levantamiento en cada cambio de armonía implícito (cada 2 compases).

4. **Texto**:
   - Insertá como System Text el tempo *Andante ♩ = 80* al inicio.
   - Insertá como Staff Text la indicación *dolce* en el compás 1.
   - Insertá marcas de ensayo A, B, C, D al inicio de los compases 1, 3, 5 y 7.

5. **Repeticiones**:
   - Insertá voltas (casilla 1 sobre compases 7–8, casilla 2 sobre compases 9–10).
   - Agregá un D.C. al Fine después de la volta 2, y colocá *Fine* sobre el compás 8.

---

### Parte 4 — Caso integrador (≈35 minutos, 25%)

**Consigna**: Creá una partitura desde cero que cumpla con las siguientes especificaciones. Llamala `APELLIDO_Nombre_S15_simulacro.mscz`.

#### Especificaciones de la partitura:

| Elemento | Especificación |
|---|---|
| **Plantilla** | Piano (gran pentagrama) |
| **Título** | "Mi primera pieza — Simulacro Interciclo" |
| **Compositor** | Tu nombre completo |
| **Tonalidad** | Fa mayor (1 bemol: Si♭) |
| **Compás** | 4/4 |
| **Tempo** | *Moderato* ♩ = 100 |
| **Estructura** | 16 compases: A (c.1–8) + B (c.9–16) |

#### Lo que DEBE contener la partitura:

1. **En el pentagrama superior (mano derecha)**:
   - Una melodía original en la tonalidad de Fa mayor, usando redondas, blancas, negras y corcheas.
   - Abarcá al menos 6 notas diferentes del ámbito Do₄–Fa₅.
   - Incluí al menos **3 alteraciones accidentales** (sostenidos, bemoles o becuadros fuera de la armadura).
   - La sección A (c.1–8) debe usar predominantemente negras y corcheas. La sección B (c.9–16) debe contrastar usando valores más largos (blancas y redondas con puntillo).
   - Incluí al menos **un tresillo** de corcheas en alguna parte de la melodía.

2. **En el pentagrama inferior (mano izquierda)**:
   - Un acompañamiento simple en negras y blancas.
   - Las notas del acompañamiento deben pertenecer a los acordes de Fa mayor (I=Fa, IV=Si♭, V=Do) y su relativo menor (vi=Re m).
   - Usá al menos una vez un acorde con bajo alterado (ej. Fa/Do, Si♭/Fa).

3. **Articulaciones y expresión**:
   - Insertá al menos **4 articulaciones diferentes** distribuidas en la melodía: acentos, staccatos, fermatas y tenutos.
   - Insertá dinámicas: empezar en *p*, crecer a *mf* con un regulador de crescendo en los compases 3–4, alcanzar *f* en el compás 9, diminuendo a *p* en los compases 15–16.
   - Agregá al menos **2 ligaduras de expresión** sobre frases melódicas.

4. **Repeticiones y estructura**:
   - La sección A (c.1–8) debe tener **barra de repetición** (inicio y fin).
   - La sección A debe tener **voltas**: casilla 1 sobre los compases 7–8, casilla 2 también sobre 7–8 (finales alternativos).
   - Agregá un **D.C. al Fine** después del compás 16. Colocá la marca *Fine* al final del compás 8 (después de la casilla 2). La pieza debe ejecutarse: A (con volta 1) → repetir A (con volta 2) → B → volver al principio → tocar A (con volta 2) → Fine.

5. **Texto y marcas**:
   - Insertá **marcas de ensayo** (A, B, C, D) al inicio de los compases 1, 5, 9 y 13.
   - Insertá el texto de expresión *cantabile* como Staff Text en el compás 1 de la mano derecha.
   - Insertá el texto de expresión *legato* como Staff Text en el compás 1 de la mano izquierda.
   - **Opcional (punto extra)**: Ingresá la letra de una canción inventada que encaje con tu melodía usando `Ctrl + L` sobre el pentagrama superior, con al menos 1 melisma de 3 notas.

6. **Entrega**:
   - Exportá y entregá **solo el PDF** (`APELLIDO_Nombre_S15_simulacro.pdf`). NO entregues el `.mscz` en esta ocasión (simulamos que el examen solo acepta PDF).
   - El archivo debe llamarse exactamente como se indica arriba.

### Entregables

- [ ] Comentario en Classroom con las respuestas de las Partes 1 y 2.
- [ ] `APELLIDO_Nombre_S15_simulacro.pdf` (exportado desde tu `.mscz`).

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Parte 1: Conceptual | 4–5 respuestas correctas, claras, con ejemplos | 2–3 correctas o sin ejemplos | ≤1 correcta |
| Parte 2: Procedimental | 7–8 atajos/rutas correctas | 4–6 correctas | ≤3 correctas |
| Parte 3: Aplicación | ≥5 de los 5 bloques completos y correctos | 3–4 bloques completos | ≤2 bloques completos |
| Parte 4: Integrador | Cumple TODAS las especificaciones; estructura A-B; repeticiones con D.C. al Fine funcionan; dinámicas y articulaciones presentes y variadas | Cumple ≥70% de las especificaciones; la pieza es reproducible pero faltan elementos | La partitura está incompleta o no se puede reproducir |
| Gestión del tiempo | Entregado dentro del límite de 90 minutos con todas las partes intentadas | Entregado a tiempo pero faltó una parte completa | No se entregó a tiempo |

---

*Basado en: MuseScore Studio 4 Handbook — Getting Started, Basics, Notation, Sound and Playback, Text (revisión integrada U1–U4)*
