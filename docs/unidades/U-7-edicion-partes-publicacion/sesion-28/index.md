# Sesión 28: Preparación de partes (particellas)

📚 Handbook → Advanced topics: Parts | Staff/Part properties | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="particella"></a> **Particella / Parte individual (part)** | La partitura que recibe CADA músico, conteniendo SOLO su instrumento. Derivada de la partitura general. No incluye los demás instrumentos. |
    | <a id="curaduria"></a> **Curaduría (curation)** | El proceso de REVISAR y AJUSTAR manualmente cada parte generada automáticamente. No es lo mismo "generar partes" (1 clic) que "preparar partes" (trabajo manual detallado). |
    | <a id="cues"></a> **Cues / Entradas guía** | Pequeñas notas en tamaño reducido que aparecen en la parte de un instrumento durante sus silencios largos, mostrando lo que otro instrumento está tocando. Sirven para que el músico sepa CUÁNDO entrar después de un silencio prolongado. |
    | <a id="pausa-multicompas"></a> **Pausa multi-compás (multi-measure rest)** | Cuando un instrumento tiene muchos compases de silencio consecutivos, NO se escriben compases individuales. Se agrupan en UN bloque con un número grande que indica cuántos compases son. |
    | <a id="transpositor"></a> **Instrumento transpositor** | Instrumento que SUENA en una altura diferente a la que está ESCRITA en la partitura. Ejemplos: Clarinete en Si♭ (suena un tono más bajo de lo escrito), Trompa en Fa (suena una quinta más baja), Saxofón alto en Mi♭ (suena una sexta mayor más baja). |
    | <a id="tono-escrito"></a> **Tono escrito (written pitch)** | La notación pensada para el INSTRUMENTISTA. En la parte de clarinete en Si♭, un Do escrito suena Si♭. El músico lee el Do y digita el Do; el instrumento produce el Si♭ automáticamente. |
    | <a id="tono-concierto"></a> **Tono de concierto (concert pitch)** | La notación en alturas REALES. El compositor escribe en tono de concierto (escucha las alturas reales). Las partes se entregan en tono ESCRITO (el músico lee lo que digita). |
    | <a id="parte-combinada"></a> **Parte combinada (merged part)** | Una parte que contiene DOS instrumentos de la misma familia (ej. Flauta I y Flauta II en la misma hoja). Se usa en ensambles escolares o para ahorrar papel. |
    | <a id="salto-pagina-parte"></a> **Salto de página en partes** | Cambio de página en una parte individual. CRÍTICO: NUNCA debe ocurrir donde el músico necesita ambas manos para tocar. Debe colocarse en silencios o notas largas que permitan voltear la página. |

???+ note "Introducción: ¿por qué las partes NO son la partitura general recortada?"
    ### El error del principiante

    Cuando generás partes automáticamente (Archivo → Partes → Generar todas), MuseScore crea una parte por cada instrumento. El principiante mira esas partes, dice "está bien", y las exporta. **ERROR.**

    Una parte individual NO es simplemente "la partitura general pero mostrando un solo pentagrama". Es un documento con sus PROPIAS reglas:

    | Característica | Partitura general | Parte individual |
    |---|---|---|
    | **Tamaño del pentagrama** | 5.0–5.5 mm (chico, para que quepan todos los instrumentos) | 7.0–7.5 mm (GRANDE, para leer desde el atril) |
    | **¿Quién la lee?** | El director (visión global) | Un músico individual (solo su línea) |
    | **Saltos de página** | Basados en la distribución visual de todos los instrumentos | Basados en dónde el MÚSICO puede voltear la página |
    | **Silencios** | Compases individuales con pausas | Pausas multi-compás agrupadas (bloque "24") |
    | **Cues** | No lleva | Incluye fragmentos de otros instrumentos durante silencios largos |
    | **Tono** | Tono de concierto (para componer) | Tono ESCRITO (para el instrumentista transpositor) |

    ### La regla de oro de las partes

    > Una parte individual BIEN hecha se reconoce porque el músico NUNCA se pierde. Las entradas después de silencios largos tienen cues, los cambios de tonalidad son visibles, las páginas voltean en silencios. Una parte MAL hecha es aquella donde el músico tiene que adivinar cuándo entrar. Si tu parte genera confusión en el ensayo, la culpa NO es del músico: es TUYA.

???+ note "Generación y curaduría: el checklist en 7 pasos"

    ### Paso 1: Generar las partes

    1. **Archivo → Partes** (o `Ctrl + Alt + P`).
    2. Clic en **"Generar todas las partes"**.
    3. MuseScore crea una parte por cada instrumento de la partitura general.

    Esto toma 1 segundo. El trabajo REAL empieza ahora.

    ### Paso 2: Cambiar el tamaño del pentagrama (PRIMERO)

    **⚠️ HACÉ ESTO ANTES DE TOCAR CUALQUIER OTRA COSA.** Si ajustás los saltos de página con pentagrama pequeño y después lo agrandás, todos los saltos se rompen y tenés que empezar de nuevo.

    1. Abrí la primera parte (doble clic en el nombre en el panel de partes).
    2. **Formato → Estilo → Tamaño**.
    3. Cambiar "Tamaño de pentagrama" a **7.5 mm**.
    4. Repetir para CADA parte.

    | Uso | Tamaño recomendado |
    |---|---|
    | Partitura general | 5.0–5.5 mm |
    | Partes individuales | 7.0–7.5 mm |

    ### Paso 3: Saltos de página estratégicos

    Activar la vista **"Diseño de página"** (el ícono de página en la barra inferior derecha, o `Ctrl + Shift + P`).

    La regla es simple pero requiere criterio: **cada salto de página debe ocurrir donde el músico tenga AL MENOS 2 segundos de silencio para voltear.**

    - **Ideal**: el salto está en un silencio de blanca con calderón, o en una pausa de varios compases.
    - **Aceptable**: el salto está en una nota larga (blanca o redonda) que el músico puede sostener con una mano mientras voltea con la otra.
    - **INACEPTABLE**: el salto está en medio de un pasaje de semicorcheas.

    Para insertar un salto de página manual:
    1. Seleccionar el compás DONDE querés que termine la página.
    2. Paleta **"Saltos y espaciadores"** → arrastrar **"Salto de página"** sobre el compás.
    3. Verificar que el compás siguiente sea un lugar cómodo para voltear.

    ### Paso 4: Pausas multi-compás

    Cuando un instrumento no toca durante 18 compases, NO escribimos 18 compases individuales de silencio. Escribimos esto:

    ```
    ┌───────────────────┐
    │        18         │  ← Número grande centrado
    │  ──────────────── │
    └───────────────────┘
    ```

    En MuseScore:
    1. **Formato → Estilo → Pausas**.
    2. Activar **"Crear pausas multi-compás"**.
    3. Configurar el **umbral mínimo**: ¿a partir de cuántos compases se agrupan? Recomendado: 2.

    ??? tip "Umbral de agrupación"
        Si ponés umbral en 2, bloques de 2+ compases de silencio se agrupan. Si ponés 4, solo silencios de 4+ compases se agrupan (los de 2–3 quedan individuales). Sé CONSISTENTE en todas las partes.

    ### Paso 5: Cues — entradas guía

    Durante silencios de más de 8 compases, el músico PIERDE LA NOCIÓN de dónde está en la obra. Necesita una GUÍA para saber cuándo entrar.

    **Cómo insertar un cue:**
    1. Identificar un silencio largo en la parte (ej. el fagot no toca del compás 24 al 38).
    2. Volver a la partitura general. Copiar una frase melódica de OTRO instrumento que suena durante ese silencio (ej. la melodía del oboe en los compases 30–34).
    3. Pegar esa frase en la PARTE del fagot, en el lugar correspondiente del silencio.
    4. Seleccionar las notas pegadas → **Propiedades** → marcar **"Notas pequeñas"**.
    5. Reducir el tamaño al 60–70%.
    6. Agregar un texto pequeño con el nombre del instrumento: "Ob." sobre el cue.
    7. En el Inspector (F8), marcar **"Excluir de la reproducción"** para que el cue no suene.

    **¿Cuándo poner cues?** Cuando el silencio es de 8+ compases. Si son 4 compases de silencio, el músico puede contarlos. Si son 24, imposible.

    ### Paso 6: Verificar transposición

    Para instrumentos transpositores (Clarinete en Si♭, Trompa en Fa, Saxofón alto en Mi♭, Trompeta en Si♭):

    - El botón **"Tono de concierto"** en la barra de herramientas debe estar **DESACTIVADO** cuando mirás la parte.
    - **Verificación**: compará la armadura de la parte del clarinete con la de la flauta. Si la obra está en Fa mayor (1 bemol) y el clarinete en Si♭ también muestra 1 bemol, ALGO ESTÁ MAL. El clarinete en Si♭ debe mostrar 1 sostenido (para que suene 1 bemol).

    | Instrumento | Transporte | Si la obra está en Do mayor, la parte muestra |
    |---|---|---|
    | Clarinete en Si♭ | Suena 1 tono ABAJO | Re mayor (2 sostenidos) |
    | Trompa en Fa | Suena 5ª justa ABAJO | Sol mayor (1 sostenido) |
    | Saxofón alto en Mi♭ | Suena 6ª mayor ABAJO | La mayor (3 sostenidos) |
    | Trompeta en Si♭ | Suena 1 tono ABAJO | Re mayor (2 sostenidos) |

    ### Paso 7: Metadatos y nombres

    1. Verificar que el **nombre del instrumento** aparezca en el primer sistema de cada página (por si las hojas se mezclan en el atril).
        - **Estilo → Cabecera y pie de página** → agregar "Nombre de instrumento".
    2. Agregar **número de página** visible.
    3. Verificar que los **números de compás** aparezcan al inicio de cada sistema.


???+ note "Partes combinadas y personalizadas"

    ### Combinar dos instrumentos en una parte

    A veces dos instrumentos de la misma familia comparten UNA sola parte (ej. Flauta I y Flauta II leen en la misma hoja).

    1. **Archivo → Partes**.
    2. Clic en **"Nueva"**.
    3. Nombrar la parte: "Flautas I y II".
    4. Seleccionar los dos pentagramas: Flauta I y Flauta II.
    5. Clic en **"Aceptar"**. La nueva parte muestra ambos pentagramas.

    ⚠️ Esto es aceptable para ensambles escolares. En contextos profesionales (orquesta sinfónica), cada músico recibe SOLO su línea.

    ### Renombrar una parte

    Si MuseScore nombró tu parte como "Pista 1" en lugar de "Violín I":
    1. En el diálogo de Partes, seleccionar la parte.
    2. Clic en **"Renombrar"**.
    3. Escribir el nombre correcto.

    ### Eliminar una parte

    Si generaste una parte que no necesitás:
    1. Seleccionar la parte en el diálogo de Partes.
    2. Clic en el ícono de **papelera** (🗑️).

    Esto NO elimina el pentagrama de la partitura general. Solo elimina la parte individual derivada.

---

## Actividad en Classroom

### Tarea: S28 — Preparación de partes (particellas)

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S28_partitura.mscz`, una partitura general para 8 instrumentos (Flauta, Oboe, Clarinete en Si♭, Fagot, Trompa en Fa, Violín I, Violín II, Violonchelo) en Fa mayor, 4/4, 48 compases, con marcas de ensayo (A–F) y dinámicas; (b) `ejercicio_S28_particellas_sucias.mscz`, una partitura para quinteto de vientos (Flauta, Oboe, Clarinete en Si♭, Trompa en Fa, Fagot) en Sol menor, 3/4, 40 compases, con las partes YA generadas automáticamente pero con errores deliberados de formato, tamaño, transposición, cues y pausas.

1. **Generación y curaduría de partes (8 instrumentos).** Abrí `ejercicio_S28_partitura.mscz`:
    - Generá todas las partes: **Archivo → Partes → Generar todas las partes**.
    - Para **CADA una de las 8 partes**, aplicá el checklist en orden:
        - Cambiar tamaño de pentagrama a **7.5 mm**. (Paso 1, ANTES que cualquier otra cosa.)
        - Revisar y ajustar **saltos de página**: cada salto debe estar en un silencio o nota larga.
        - Configurar **pausas multi-compás** (umbral: 2 compases).
        - Insertar **cues** en silencios de 8+ compases (nombre del instrumento guía visible).
        - Verificar **transposición**: el Clarinete en Si♭ y la Trompa en Fa en tono ESCRITO (botón de concierto DESACTIVADO).
        - Verificar que las **marcas de ensayo** y números de compás sean visibles.
        - Verificar que el **nombre del instrumento** aparezca en cada página.
    - Exportá TODAS las 8 partes como PDFs individuales: `APELLIDO_S28_parte_Flauta.pdf`, etc.

2. **Diagnóstico y corrección de partes sucias.** Abrí `ejercicio_S28_particellas_sucias.mscz`:
    - **Primero, DIAGNOSTICÁ** (sin tocar nada): abrí cada una de las 5 partes y anotá TODOS los errores que encontrés. Se espera que encuentres al menos 7 tipos de errores.
    - **Después, CORREGÍ**: aplicá el checklist completo para que las 5 partes queden profesionales.
    - **Documentá**: para cada error, explicá en tu comentario de Classroom qué estaba mal y cómo lo corregiste.
    - Exportá las 5 partes corregidas como PDF.

3. **Cues especiales.** En la partitura de 8 instrumentos, identificá el silencio más largo de cada instrumento (no necesariamente el mismo para todos). Insertá cues relevantes al menos en las 3 partes con los silencios más largos.

4. **Reflexión.** En Classroom, respondé:
    - ¿Cuánto tiempo te llevó corregir UNA parte vs. generarla automáticamente? ¿Te sorprendió la diferencia?
    - ¿Cuál fue el error más difícil de detectar en las partes sucias? ¿Por qué era difícil?
    - Si fueras el director de un ensamble y un músico se pierde en el ensayo porque su parte estaba mal formateada, ¿de quién es la responsabilidad? Justificá tu respuesta.

### Entregables

- [ ] 8 PDFs de partes individuales de la partitura de 8 instrumentos (`APELLIDO_S28_parte_Flauta.pdf`, etc.)
- [ ] 5 PDFs de partes corregidas del quinteto de vientos
- [ ] Comentario en Classroom con: (a) diagnóstico de errores del quinteto (mínimo 7 tipos de errores detectados), (b) respuestas a las 3 preguntas de reflexión.

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Generación de partes (8 instrumentos) | 8 partes generadas; todas con pentagrama 7.5 mm; saltos correctos; pausas multi-compás; cues en al menos 3 partes | 6–7 partes correctas | ≤5 partes |
| Transposición | Clarinete y Trompa en tono escrito en TODAS sus partes | Solo un instrumento correcto | Ambos en tono de concierto |
| Diagnóstico (quinteto) | ≥7 tipos de errores identificados y documentados ANTES de corregir | 5–6 errores identificados | ≤4 errores |
| Corrección (quinteto) | 5 partes corregidas con checklist completo; todos los errores resueltos | Mayoría de errores corregidos pero quedan ≥2 | Quedan ≥5 errores sin corregir |
| Exportación | Todas las partes exportadas como PDF individuales con nombres descriptivos | Mayoría exportada correctamente | Archivos sin nombre descriptivo |
| Reflexión | 3 respuestas con comprensión de la diferencia entre generar y preparar partes | 2 respuestas correctas | ≤1 respuesta correcta |

---

*Basado en: MuseScore Studio 4 Handbook — Advanced topics: Parts, Staff/Part properties | https://handbook.musescore.org*
