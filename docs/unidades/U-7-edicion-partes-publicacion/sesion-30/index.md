# Sesión 30: Control de calidad y revisión profesional

📚 Handbook → Advanced topics: Score Comparison, Accessibility | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="qc"></a> **Control de calidad (QC / Quality Control)** | Proceso sistemático de REVISIÓN de una partitura ANTES de publicarla o entregarla. Busca detectar errores de notación, formato, metadatos y accesibilidad. |
    | <a id="ojo-editorial"></a> **Ojo editorial** | Habilidad desarrollada con práctica para detectar errores sutiles en partituras: una alteración incorrecta, un espaciado inconsistente, una colisión de elementos. Los editores profesionales entrenan este ojo durante años. |
    | <a id="score-comparison"></a> **Comparación de partituras (Score Comparison)** | Herramienta de MuseScore que compara DOS archivos y muestra sus diferencias visualmente. Similar al "git diff" pero para partituras. |
    | <a id="diferencia-codificada"></a> **Diferencia codificada por color** | En Score Comparison: VERDE = eliminado (estaba en A, no en B). ROJO = agregado (estaba en B, no en A). AZUL = modificado (diferente entre A y B). |
    | <a id="fe-errata"></a> **Fe de erratas (errata list)** | Documento publicado por una editorial listando los errores encontrados en una edición YA impresa. Es una admisión pública de error. Muy vergonzoso. Mejor prevenir que curar. |
    | <a id="accesibilidad"></a> **Accesibilidad en partituras** | Diseñar partituras que puedan ser LEÍDAS por cualquier músico en cualquier condición: visión reducida, baja iluminación, impresión blanco y negro, lectura en tablet. |
    | <a id="contraste"></a> **Contraste** | Diferencia visual entre un elemento y su fondo. Texto negro sobre blanco = alto contraste (✔). Texto gris claro sobre blanco = bajo contraste (✘). Fundamental para legibilidad. |
    | <a id="colision"></a> **Colisión** | Cuando dos elementos de la partitura se SUPERPONEN visualmente. Ejemplo: una dinámica que tapa una nota, una ligadura que cruza un becuadro. Siempre es un error de formato. |
    | <a id="proofreader"></a> **Corrector de pruebas (proofreader)** | Profesional cuyo ÚNICO trabajo es encontrar errores en partituras antes de su publicación. Un proofreader profesional revisa 10–20 páginas por DÍA. No por hora. Por DÍA. |

???+ note "Introducción: ¿por qué revisar es la habilidad más subestimada?"

    ### El mito del "terminé"

    Terminaste de escribir tu partitura. Pusiste la última nota. Las dinámicas están. Las partes fueron generadas. Todo está listo.

    **NO. Ahora EMPIEZA el trabajo más importante: la revisión.**

    El 90% de los estudiantes entrega su partitura SIN REVISAR. El resultado:
    - Notas equivocadas que el director detecta en el primer ensayo.
    - Saltos de página que hacen que los músicos se pierdan.
    - Metadatos vacíos (el PDF aparece como "Untitled").
    - Dinámicas superpuestas que son ilegibles.

    ### La diferencia entre un borrador y una publicación

    | Borrador | Publicación |
    |---|---|
    | "Creo que está bien." | "SÉ que está bien porque lo revisé 3 veces." |
    | Errores de nota: probablemente. | Errores de nota: 0 (idealmente). |
    | Formato: "lo que MuseScore puso por defecto." | Formato: decisiones INTENCIONALES. |
    | "Ya fue, lo entrego así." | "Voy a imprimirlo y revisarlo una vez más." |

    > **"El mejor editor de partituras no es el que escribe más rápido. Es el que revisa MEJOR."**

???+ note "El checklist de control de calidad editorial"

    Revisar una partitura NO es leerla de corrido y esperar que los errores "salten a la vista". Es un proceso en CAPAS. Cada capa se enfoca en UNA categoría de posibles errores.

    Imprimí esta checklist y usala CADA VEZ que termines una partitura.

    ### A. NOTACIÓN — ¿está bien escrito lo que el músico lee?

    - [ ] ¿Todas las notas tienen la altura correcta? Reproducí CADA voz por separado (solapar con el mezclador).
    - [ ] ¿Todas las alteraciones son correctas? ¿Hay enarmonías incorrectas? (Sol♯ en lugar de La♭ en un contexto de Fa menor.)
    - [ ] ¿Los valores rítmicos suman correctamente? MuseScore no te deja exceder, pero podés tener compases INCOMPLETOS.
    - [ ] ¿Las pausas están en la posición vertical correcta? (Pausa de blanca en 3ª línea, de redonda colgando de la 4ª.)
    - [ ] ¿Las ligaduras de expresión (slur) y de prolongación (tie) están correctamente distinguidas?
    - [ ] ¿Los matices (pp, mf, ff) tienen sentido musical?
    - [ ] ¿Los reguladores (cresc./dim.) tienen un punto de llegada claro?

    ### B. FORMATO — ¿está bien presentado visualmente?

    - [ ] ¿Los saltos de página están en lugares donde el músico puede voltear? (ESTO ES LO MÁS IMPORTANTE.)
    - [ ] ¿Los sistemas están balanceados visualmente? (No 1 compás solitario al final de una página.)
    - [ ] ¿Hay colisiones? (Dinámicas que tapan notas, letras que se superponen, ligaduras que cruzan alteraciones.)
    - [ ] ¿El espaciado es consistente? (Compases con muchas notas NO deben estar aplastados.)
    - [ ] ¿El tamaño de pentagrama es correcto? (5.5 mm full score, 7.5 mm partes.)
    - [ ] ¿Los márgenes son adecuados? (Mínimo 10–12 mm en todos los lados.)

    ### C. METADATOS Y TEXTO — ¿está completa la información?

    - [ ] ¿El título es correcto y sin errores de ortografía?
    - [ ] ¿El compositor está acreditado?
    - [ ] ¿El copyright está presente?
    - [ ] ¿Las indicaciones de tempo usan ITALIANO estándar? (Allegro, no "rápido".)
    - [ ] ¿No hay errores de ortografía en NINGÚN texto? (Indicaciones, letras, títulos de sección.)

    ### D. PARTES INDIVIDUALES — ¿funcionan para cada músico?

    - [ ] ¿Cada parte está en el TONO CORRECTO? (Transpositores: tono ESCRITO.)
    - [ ] ¿Las pausas multi-compás están agrupadas y numeradas?
    - [ ] ¿Los cues son visibles y tienen nombre de instrumento?
    - [ ] ¿Los números de compás coinciden con la partitura general?
    - [ ] ¿Las marcas de ensayo están en los mismos lugares?

    ### E. ACCESIBILIDAD — ¿puede leerlo CUALQUIER músico?

    - [ ] ¿El contraste es suficiente? (Texto negro sobre blanco. NO grises claros.)
    - [ ] ¿El tamaño de fuente es legible? (Mínimo 10 pt para dinámicas, 12 pt para tempo.)
    - [ ] ¿La partitura funciona en BLANCO Y NEGRO? (Si usaste colores, ¿se distinguen las voces sin color?)
    - [ ] ¿Los elementos importantes están en lugares VISIBLES? (No escondidos detrás de otras marcas.)

    !!! tip "El paso que NADIE hace"
        **Imprimí la partitura.** Leela en papel. Los errores que ignoraste en pantalla SALTAN A LA VISTA en papel. Esto no es superstición: es cómo funciona la percepción visual humana. En pantalla hacés scroll y zoom. En papel ves la página completa. Son dos experiencias de lectura completamente diferentes.

???+ note "Score Comparison: el 'diff' de partituras"

    MuseScore incluye una herramienta para comparar dos versiones de la misma partitura y visualizar exactamente QUÉ cambió.

    ### Cómo usar Score Comparison

    1. **Herramientas → Comparar partituras**.
    2. Seleccionar el PRIMER archivo (versión "antes"): `ejercicio_S30_comparacion_a.mscz`.
    3. Seleccionar el SEGUNDO archivo (versión "después"): `ejercicio_S30_comparacion_b.mscz`.
    4. MuseScore genera una NUEVA partitura que muestra las diferencias.

    ### Código de colores

    | Color | Significado | Ejemplo |
    |---|---|---|
    | 🟢 **Verde** | Presente en A pero NO en B (eliminado) | Una nota que existía en la versión A y fue borrada en la B |
    | 🔴 **Rojo** | Presente en B pero NO en A (agregado) | Una dinámica nueva que no estaba en la versión A |
    | 🔵 **Azul** | Diferente entre A y B (modificado) | Una nota que era Fa♮ en A y ahora es Fa♯ en B |

    ### ¿Qué detecta? ¿Qué NO detecta?

    | ✅ SÍ detecta | ❌ NO detecta |
    |---|---|
    | Notas agregadas, eliminadas o modificadas | Cambios de márgenes o espaciado |
    | Alteraciones cambiadas | Cambios de tamaño de pentagrama |
    | Dinámicas, articulaciones, texto modificados | Cambios de fuente tipográfica |
    | Compases agregados o eliminados | Cambios de posición visual de elementos (si la nota es la misma) |
    | Cambios de tempo | Saltos de página o de sistema |

    ### ¿Cuándo usar Score Comparison?

    - **Trabajo colaborativo**: un colega modificó tu partitura. ¿Qué cambió exactamente?
    - **Control de versiones**: tenés "MiObra_v2.mscz" y "MiObra_v3.mscz". ¿Qué diferencias hay?
    - **Detección de errores**: comparar tu versión con una versión de referencia para encontrar discrepancias.

    > Insertar captura de MuseScore mostrando el resultado de Score Comparison: una partitura con notas en verde, rojo y azul, y la leyenda de colores visible.

???+ note "Accesibilidad: diseñar partituras para TODOS los músicos"

    Cuando hablamos de accesibilidad en partituras, no hablamos solo de lectores de pantalla para personas ciegas. Hablamos de que CUALQUIER músico pueda leer tu partitura en CUALQUIER condición.

    ### Los 4 pilares de la accesibilidad en partituras

    #### 1. TAMAÑO

    | Edad / Condición | Tamaño mínimo recomendado |
    |---|---|
    | Músico joven (15–25) | Pentagrama 7.0 mm |
    | Músico adulto (40+) | Pentagrama 7.5–8.0 mm |
    | Baja iluminación (atril con luz tenue) | Pentagrama 8.0 mm |
    | Lectura en tablet (iPad 10") | Pentagrama 7.5 mm |

    **Regla**: si dudás entre dos tamaños, elegí el MÁS GRANDE. Un pentagrama grande nunca molestó a nadie. Un pentagrama chico SÍ.

    #### 2. CONTRASTE

    - **Texto negro (#000000) sobre fondo blanco (#FFFFFF)** → contraste MÁXIMO. ✔
    - **Texto gris (#999999) sobre fondo blanco** → contraste INSUFICIENTE. ✘
    - Si usás colores para distinguir voces en una partitura coral (SATB), asegurate de que TAMBIÉN se distingan por tamaño o estilo. Si alguien imprime en blanco y negro, las voces deben seguir siendo diferenciables.

    #### 3. FUENTES

    - Para indicaciones de tempo y texto: usar fuentes CLARAS y de alto contraste.
    - Fuentes seguras: FreeSerif, FreeSans, Times New Roman, Arial.
    - Fuentes a EVITAR: decorativas, script, caligráficas (difíciles de leer a distancia).
    - **NUNCA usar Comic Sans en una partitura profesional.** Simplemente no.

    #### 4. BLANCO Y NEGRO

    Muchas partituras se imprimen en impresoras blanco y negro. Si tu notación depende de COLORES para comunicar algo (voces, matices, secciones), esa información se PIERDE completamente en B&N.

    **Solución**: usar múltiples codificaciones. Si usás color para la voz de soprano, también ponela en un tamaño diferente o con un estilo de nota distinto.

    !!! warning "El error del color"
        Si tu partitura tiene "las notas del director en ROJO y las del estudiante en AZUL", cuando alguien la imprima en blanco y negro, AMBAS serán negras. El resultado: el estudiante toca las notas del director. Desastre.

---

## Actividad en Classroom

### Tarea: S30 — Control de calidad y revisión profesional

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S30_revision.mscz`, una partitura para trío (Violín, Violonchelo, Piano) en Re menor (1 bemol), 3/4, 40 compases, con al menos 15 errores deliberados distribuidos en las 5 categorías del checklist (notación, formato, metadatos, partes, accesibilidad); (b) `ejercicio_S30_comparacion_a.mscz` y (c) `ejercicio_S30_comparacion_b.mscz`, dos versiones de un minueto para cuarteto de cuerdas en Do mayor, 3/4, 32 compases, con 15–20 diferencias entre ambas.

1. **Auditoría completa de `ejercicio_S30_revision.mscz`.** Usando el checklist de 5 categorías (imprimilo si podés):
    - Revisá la partitura por CAPAS: primero solo NOTACIÓN, después solo FORMATO, después solo METADATOS, después solo PARTES, después solo ACCESIBILIDAD.
    - **Documentá CADA error** que encuentres. Para cada error, indicá:
      - **Compás / ubicación** (ej. "compás 12, Violín, 3er tiempo").
      - **Categoría** (Notación / Formato / Metadatos / Partes / Accesibilidad).
      - **Descripción** (qué está mal).
      - **Corrección propuesta** (cómo debería ser).
    - Se espera que encuentres al menos 12 de los 15+ errores.
    - **IMPORTANTE**: no corrijas el archivo todavía. Primero diagnosticá TODO. Después corregí.

2. **Corrección editorial.** Después de diagnosticar TODOS los errores:
    - Corregí la partitura en MuseScore.
    - Guardá la versión corregida como `APELLIDO_S30_revision_corregida.mscz`.
    - Exportá como PDF: `APELLIDO_S30_revision_corregida.pdf`.

3. **Score Comparison — el minueto.** Ejecutá la herramienta de comparación:
    - **Herramientas → Comparar partituras**.
    - Primer archivo: `ejercicio_S30_comparacion_a.mscz`.
    - Segundo archivo: `ejercicio_S30_comparacion_b.mscz`.
    - Examiná la partitura resultante. Clasificá las diferencias en una tabla:

      | Compás | Instrumento | Tipo (Agregado / Eliminado / Modificado) | Descripción |
      |---|---|---|---|
      | 5 | Violín I | Modificado | Fa♮ cambió a Fa♯ |
      | 8 | Viola | Eliminado | Ligadura de expresión borrada |
      | 12 | Violonchelo | Agregado | Nueva dinámica *mf* |
      | ... | ... | ... | ... |

    - Guardá el resultado como `APELLIDO_S30_comparacion_resultado.mscz`.
    - Exportá como PDF: `APELLIDO_S30_comparacion_resultado.pdf`.

4. **Informe de accesibilidad.** Sobre la partitura `ejercicio_S30_revision.mscz` (la original con errores, ANTES de corregir):
    - Evaluá la partitura según los 4 pilares de accesibilidad (tamaño, contraste, fuentes, B&N).
    - Escribí un breve informe (una página máximo) con:
      - ¿Qué elementos violan los principios de accesibilidad?
      - ¿Qué mejorarías?
      - ¿Cómo se leería esta partitura impresa en blanco y negro? ¿Qué información se perdería?

5. **Reflexión sobre el control de calidad.** En Classroom, respondé:
    - ¿Cuántos errores encontraste en total? ¿Cuál fue el más DIFÍCIL de detectar y por qué?
    - ¿Qué categoría del checklist te resultó más fácil de revisar? ¿Cuál más difícil?
    - Si tuvieras que contratar a alguien para revisar tus partituras (un proofreader), ¿qué cualidades buscarías? ¿Qué te daría CONFIANZA en su trabajo?
    - ¿Creés que el control de calidad es "trabajo extra" o es PARTE del trabajo de crear una partitura? Justificá.

### Entregables

- [ ] Lista de errores detectados en `ejercicio_S30_revision.mscz` (mínimo 12), con compás, categoría, descripción y corrección propuesta.
- [ ] `APELLIDO_S30_revision_corregida.mscz` y `APELLIDO_S30_revision_corregida.pdf`
- [ ] `APELLIDO_S30_comparacion_resultado.mscz` y `APELLIDO_S30_comparacion_resultado.pdf`
- [ ] Tabla de diferencias de Score Comparison (mínimo 15 entradas, clasificadas por tipo).
- [ ] Informe de accesibilidad (una página máximo).
- [ ] Comentario en Classroom con las 4 respuestas de reflexión.

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Detección de errores | ≥12 errores detectados y clasificados correctamente | 8–11 errores | ≤7 errores |
| Categorización | Cada error en la categoría correcta del checklist | Mayoría correcta | Categorías arbitrarias |
| Corrección | Errores corregidos correctamente; partitura final profesional | La mayoría corregidos pero quedan +2 errores | Quedan ≥5 errores o se introdujeron nuevos |
| Score Comparison | Tabla con ≥15 diferencias clasificadas (agregado/eliminado/modificado) | 10–14 diferencias | ≤9 diferencias |
| Accesibilidad | Informe que identifica violaciones según los 4 pilares (tamaño, contraste, fuentes, B&N) | 3 de 4 pilares cubiertos | ≤2 pilares |
| Reflexión | 4 respuestas con profundidad y criterio editorial | 3 respuestas correctas | ≤2 respuestas |

---

*Basado en: MuseScore Studio 4 Handbook — Advanced topics: Score Comparison, Accessibility | https://handbook.musescore.org*
