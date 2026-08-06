# Sesión 21: Notación para ensambles grandes

📚 Handbook → Advanced topics: Parts, Staff/Part properties | Formatting: Brackets and braces, Page layout concepts | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="partitura-general"></a> **Partitura general (full score)** | La partitura que contiene TODOS los instrumentos de una obra, cada uno en su pentagrama individual, apilados verticalmente y alineados temporalmente. El director la usa para tener una visión completa de la obra. También se llama *conductor's score*. |
    | <a id="parte"></a> **Parte individual (part)** | La partitura que recibe CADA músico, conteniendo SOLO su instrumento. Derivada de la partitura general. El violinista no necesita ver lo que hace el fagot; solo necesita su parte. |
    | <a id="sistema"></a> **Sistema (system)** | Un conjunto de pentagramas que se tocan simultáneamente y están unidos por una barra vertical al inicio. En una partitura general, cada "renglón" horizontal que agrupa a todos los instrumentos es un sistema. |
    | <a id="corchete"></a> **Corchete / Bracket** | Línea vertical gruesa (tipo "[" corchete cuadrado) que agrupa pentagramas de una misma FAMILIA de instrumentos en la partitura general. Ejemplo: todos los violines con un corchete, todas las maderas con otro corchete. Los brackets ORGANIZAN visualmente la partitura. |
    | <a id="llave"></a> **Llave / Brace** | Línea vertical con forma de "{" (llave de agrupación) que une dos o más pentagramas de un MISMO instrumento. El ejemplo clásico: los dos pentagramas del piano (mano derecha e izquierda) unidos por una llave. También se usa para el arpa, el órgano, o la celesta. |
    | <a id="barra-compas"></a> **Barra de compás (barline)** | Las líneas verticales que dividen los compases. En las partituras generales, las barras de compás pueden ser CONTINUAS (cruzan todos los pentagramas del sistema) o DISCONTINUAS (cada familia tiene sus propias barras). Las barras continuas son el estándar moderno para partituras orquestales. |
    | <a id="pentagrama-oculto"></a> **Pentagrama oculto (hidden staff)** | Pentagrama que existe en la partitura pero NO se muestra en ciertos sistemas donde el instrumento no toca. MuseScore puede ocultar automáticamente los pentagramas vacíos para ahorrar espacio vertical. Es una práctica estándar en partituras orquestales. |
    | <a id="salto-sistema"></a> **Salto de sistema (system break)** | Instrucción que fuerza a la partitura a comenzar un NUEVO sistema (nuevo renglón) en ese punto. Se usa cuando el sistema actual está demasiado lleno, para separar secciones musicales visualmente, o para que un cambio de tempo/armadura/compás coincida con el inicio de un sistema. |
    | <a id="salto-pagina"></a> **Salto de página (page break)** | Fuerza una nueva página. Manual. Crítico para las partes individuales: un músico NO puede dar vuelta la página en medio de un pasaje rápido. Los saltos de página deben colocarse donde el músico tenga al menos 2–3 segundos de silencio para voltear. |
    | <a id="formato-pagina"></a> **Formato de página (page layout)** | La configuración general de la partitura: tamaño de papel (A4, Carta, 9×12 pulgadas para partes orquestales), márgenes, espaciado de pentagramas, tamaño de fuente, distancia entre sistemas. Un buen formato de página hace la diferencia entre una partitura profesional y una "de principiante". |
    | <a id="espaciado"></a> **Espaciado de pentagramas (staff spacing)** | Distancia vertical entre pentagramas adyacentes. En partituras con MUCHOS instrumentos (orquesta sinfónica: 20+ pentagramas), el espaciado debe ser ajustado pero legible. En partes individuales, el espaciado debe ser GENEROSO para que el músico pueda anotar digitaciones, arcos y matices. |
    | <a id="nombre-instrumento"></a> **Nombre de instrumento (instrument name)** | Etiqueta que aparece a la izquierda del primer sistema de cada página identificando el instrumento. Puede ser completo ("Violín I") o abreviado ("Vln. I") en sistemas subsiguientes. En partes orquestales profesionales, el nombre del instrumento aparece en CADA página por si las hojas se mezclan. |
    | <a id="orden-instrumental"></a> **Orden instrumental (instrument order)** | La secuencia en que los instrumentos aparecen en la partitura general, de arriba hacia abajo. El orden estándar orquestal es: maderas (flautas, oboes, clarinetes, fagotes) → metales (trompas, trompetas, trombones, tuba) → percusión → arpa/piano/celesta → cuerdas (violines I, violines II, violas, cellos, contrabajos). Este orden NO es arbitrario: sigue la disposición física tradicional de la orquesta en el escenario. |
    | <a id="marcador-ensayo"></a> **Marcador de ensayo (rehearsal mark)** | Letra o número colocado sobre el pentagrama para marcar puntos de referencia en la partitura. El director dice: "vamos desde la letra D". Imprescindible en obras largas o para ensambles grandes. En MuseScore se inserta con `Ctrl + M`. |

???+ note "Partitura general vs. partes individuales: dos documentos, un propósito"

    ### La partitura general (full score)

    Es el "plano maestro" del edificio. El director la usa para verlo TODO simultáneamente. Características:

    - **TODOS los instrumentos** apilados verticalmente en cada sistema.
    - **Pentagramas pequeños** (tamaño reducido) para que quepan todos en una página. Un tamaño típico de pentagrama en partitura general orquestal es 4–5 mm de altura (vs. 7–8 mm para partes individuales).
    - **Barras de compás continuas** que cruzan todos los pentagramas.
    - **Brackets y llaves** organizando las familias instrumentales.
    - **Pentagramas vacíos ocultos** cuando un instrumento no toca durante sistemas completos.
    - Los **nombres de instrumento** aparecen completos en la primera página y abreviados en las siguientes.

    ### Las partes individuales (parts)

    Es lo que va al atril de CADA músico. Características:

    - **UN solo instrumento** por parte (o un par, ej. Flauta I y II juntas en la misma parte).
    - **Tamaño de pentagrama GRANDE** (7–8 mm) para lectura fácil a distancia.
    - **Márgenes generosos** para anotaciones del músico.
    - **Saltos de página estratégicos:** NUNCA en medio de un pasaje rápido o en un silencio demasiado corto para voltear.
    - **Pausas multi-compás** (compases de silencio agrupados en un solo bloque con un número).
    - **Indicaciones de otros instrumentos** (cues) en letra pequeña durante silencios largos: "Trompeta" o "Ob." escrito en la parte para que el músico sepa cuándo entrar.

    !!! tip "La regla de oro de las partes"
        Una parte individual BIEN hecha se reconoce porque el músico NUNCA se pierde. Las entradas después de silencios largos tienen marcas de ensayo, los cambios de tonalidad son visibles, las páginas voltean en silencios. Una parte MAL hecha es aquella donde el músico tiene que adivinar cuándo entrar. Si tu parte genera confusión en el ensayo, la culpa NO es del músico: es TUYA.

    > Insertar comparación lado a lado: (izquierda) una página de partitura general orquestal mostrando 15 pentagramas apilados con brackets, (derecha) una parte individual de violín I mostrando el mismo pasaje ampliado y con números de compás.

???+ note "Brackets, llaves y barras de compás: la gramática visual de la partitura"

    La partitura general tiene una SINTAXIS VISUAL. Los símbolos de agrupación no son decorativos: comunican JERARQUÍA y FAMILIA.

    ### Tipos de agrupadores

    | Símbolo | Nombre | Uso | Significado |
    |---|---|---|---|
    | **`[`** | **Bracket / Corchete** | Agrupa instrumentos de la misma familia (todas las maderas, todos los metales, todas las cuerdas superiores) | "Estos instrumentos pertenecen al MISMO GRUPO tímbrico" |
    | **`{`** | **Brace / Llave** | Agrupa pentagramas de un MISMO instrumento (piano mano derecha + izquierda, arpa, órgano) o de instrumentos idénticos (Violín I + Violín II) | "Estos pentagramas son PARTE DEL MISMO INSTRUMENTO" |
    | **`└──`** | **Sub-bracket** | Agrupa sub-familias dentro de una familia (flauta I + II + flautín dentro de las maderas) | "Estos son instrumentos HERMANOS dentro de la familia" |

    ### Estructura visual estándar de una partitura orquestal moderna

    ```
    ┌─────────────────────────────────┐
    │ Piccolo                          │
    │ 2 Flautas                        │ ← Bracket de maderas [ 
    │ 2 Oboes                          │
    │ Corno Inglés                     │
    │ 2 Clarinetes en Si♭              │
    │ Clarinete Bajo                   │
    │ 2 Fagotes                        │
    │ Contrafagot                      │
    ├─────────────────────────────────┤
    │ 4 Trompas en Fa                  │ ← Bracket de metales [
    │ 3 Trompetas en Si♭               │
    │ 2 Trombones Tenores              │
    │ Trombón Bajo + Tuba              │
    ├─────────────────────────────────┤
    │ Timbales                         │ ← Bracket de percusión [
    │ Percusión (3 ejecutantes)        │
    ├─────────────────────────────────┤
    │ Arpa                             │ ← Sin bracket (solista)
    │ Piano / Celesta                  │   o bracket propio
    ├─────────────────────────────────┤
    │ Violines I                     ┐ │
    │ Violines II                    ├─│ ← Bracket de cuerdas [
    │ Violas                         │ │   + Sub-brackets internos
    │ Violonchelos                   ┘ │
    │ Contrabajos                      │
    └─────────────────────────────────┘
    ```

    ### Cómo insertar brackets y llaves en MuseScore

    1. **Agregar un bracket a un grupo de pentagramas:**
       - Seleccionar el primer pentagrama del grupo que querés agrupar.
       - Ir a la paleta **Líneas → Brackets** (o **Añadir → Corchetes/llaves**).
       - Arrastrar el bracket sobre el pentagrama. Se extiende automáticamente para cubrir todos los pentagramas del grupo si están configurados como tal.
       - Para extender manualmente: hacer clic en el bracket y arrastrar el manejador inferior hacia abajo.
    2. **Agregar una llave (brace):**
       - Funciona igual que el bracket. Seleccionar el pentagrama y arrastrar la llave desde la paleta.
       - Típicamente usado para unir los dos pentagramas del piano o del arpa.
    3. **Editar propiedades del bracket:**
       - Clic derecho en el bracket → **Propiedades del bracket**.
       - Se puede cambiar: si abarca todo el sistema o solo el grupo, el estilo visual, si se repite en cada sistema o solo al inicio.

    ### Barras de compás: continuas vs. discontinuas

    En MuseScore, por defecto las barras de compás son CONTINUAS (cruzan todos los pentagramas). En música orquestal moderna, esto es lo esperado.

    Si querés barras DISCONTINUAS (cada familia tiene sus propias barras, separadas visualmente):
    1. Ir a **Formato → Estilo → Barras de compás**.
    2. Desmarcar "Barras de compás continuas" o ajustar "Extender barras de compás a través de los grupos de pentagramas".
    3. Esta opción es más común en música coral (SATB) o en ediciones históricas.

    > Insertar captura de MuseScore mostrando la paleta de brackets/llaves y una partitura con los brackets aplicados: maderas agrupadas con `[`, piano con `{`, cuerdas con `[`.

???+ note "Generación y edición de partes individuales"

    Una de las funciones más potentes de MuseScore es la generación automática de partes. Pero "automática" NO significa "correcta sin revisión". La generación automática requiere CURACIÓN manual.

    ### Generar partes desde la partitura general

    1. **Abrir el diálogo de partes**: **Archivo → Partes...** (o `Ctrl + Alt + P`).
    2. **Generar partes automáticamente**: MuseScore crea una parte por cada instrumento en la partitura general. Hacé clic en "Generar" o "Generar todas las partes".
    3. **Personalizar partes**: Podés crear partes compuestas (ej. "Flauta I + II" en una sola parte) o renombrar partes. También podés crear partes para combinaciones específicas (ej. "Maderas — ensayo").
    4. **Abrir una parte**: Hacé doble clic en una parte para abrirla en una pestaña independiente.

    ### Editar una parte individual (CRÍTICO)

    La parte generada automáticamente es un PUNTO DE PARTIDA, no un producto final.

    **Checklist de edición de partes:**

    - [ ] **Tamaño del pentagrama**: ¿Es legible a distancia? En partes individuales, aumentar el tamaño a 7.0–8.0 mm (Formato → Estilo → Tamaño de pentagrama).
    - [ ] **Saltos de página**: ¿Las páginas voltean en silencios? Revisar CADA salto de página. Si un músico tiene que voltear en medio de una semicorchea, mover el salto de página.
    - [ ] **Pausas multi-compás**: ¿Los silencios largos están agrupados? Seleccionar los compases de silencio → Formato → Estilo → Pausas → marcar "Crear pausas multi-compás". MuseScore las agrupa automáticamente.
    - [ ] **Números de compás**: ¿Son visibles y legibles? En partes, los números de compás DEBEN aparecer al inicio de cada sistema.
    - [ ] **Marcas de ensayo**: ¿Están sincronizadas con la partitura general? Las marcas de ensayo (letras/números) son lo ÚNICO que permite al director y a los músicos comunicarse rápidamente. Si la letra D en la parte de violín no coincide con la letra D en la partitura general, el ensayo es un caos.
    - [ ] **Indicaciones de tempo y dinámica**: ¿Se heredaron correctamente desde la partitura general? Verificá que los matices, reguladores y cambios de tempo aparezcan.
    - [ ] **Transposición**: Para instrumentos transpositores, ¿la parte está en tono ESCRITO (no de concierto)? Activá/desactivá el botón de tono de concierto para verificar.
    - [ ] **Cues (entradas de otros instrumentos)**: Durante silencios de más de 8 compases, agregar cues en tamaño pequeño mostrando la melodía de otro instrumento para que el músico sepa cuándo entrar. En MuseScore, los cues se agregan manualmente: copiar las notas del otro pentagrama, pegarlas en la parte y reducir su tamaño.

    ### Pausas multi-compás

    Cuando un instrumento tiene, digamos, 47 compases de silencio, NO se escriben 47 compases de silencios individuales. Se agrupan en un solo bloque:

    ```
    ┌───────────────────┐
    │        47         │  ← Número grande centrado sobre el bloque de pausas multi-compás
    │  ──────────────── │
    └───────────────────┘
    ```

    En MuseScore, esto se activa automáticamente al generar partes, pero podés ajustarlo:
    - **Formato → Estilo → Pausas → Pausas multi-compás**.
    - Umbral mínimo: ¿a partir de cuántos compases se agrupan? (Típicamente 2 o 3).
    - Numeración: sí/no, posición.

    > Insertar captura de una parte de trombón en MuseScore mostrando: pausas multi-compás agrupadas (bloque con número "24"), cues en tamaño pequeño ("Trompeta"), marcas de ensayo (letra "C"), y un salto de página en un silencio de blanca con calderón.

???+ note "Formato de página para partituras profesionales"

    ### Tamaño de papel

    | Uso | Tamaño estándar | Dimensiones |
    |---|---|---|
    | Partitura general orquestal (estudio) | A3 o Tabloide (11×17") | 297×420 mm o 11×17 pulgadas |
    | Partitura general orquestal (reducción) | A4 o Carta | 210×297 mm o 8.5×11" |
    | Partes individuales orquestales | 9×12 pulgadas (Quarto) | 229×305 mm |
    | Partituras de banda / ensamble escolar | Carta o A4 | 8.5×11" o 210×297 mm |
    | Lead sheet / cifrado | Carta o A4 | 8.5×11" o 210×297 mm |

    !!! tip "Para este curso: usá SIEMPRE Carta o A4"
        Las partes en tamaño concierto (9×12") son para orquestas profesionales. Para el curso, A4 o Carta es perfecto.

    ### Configuración recomendada en MuseScore para una partitura general de 6–12 instrumentos

    | Parámetro | Valor recomendado | Dónde se configura |
    |---|---|---|
    | Tamaño de página | A4 (o Carta) | Formato → Configuración de página |
    | Márgenes | Superior: 12 mm, Inferior: 10 mm, Izquierdo: 10 mm, Derecho: 8 mm | Formato → Configuración de página |
    | Tamaño de pentagrama (full score) | 5.0–5.5 mm | Formato → Estilo → Tamaño |
    | Tamaño de pentagrama (partes) | 7.0–7.5 mm | Formato → Estilo → Tamaño (editar CADA parte) |
    | Distancia entre sistemas (full score) | 6.0–8.0 mm | Formato → Estilo → Página |
    | Distancia entre pentagramas (full score) | 3.0–4.0 mm | Formato → Estilo → Pentagrama |
    | Fuente de texto | FreeSerif o Edwin (por defecto) | Formato → Estilo → Estilos de texto |
    | Tamaño de fuente de matices | 10–11 pt | Formato → Estilo → Estilos de texto → Dinámicas |
    | Tamaño de fuente de tempo | 12–13 pt | Formato → Estilo → Estilos de texto → Tempo |

    ### Ocultar pentagramas vacíos

    En una partitura con 15 instrumentos, si la sección de cuerdas no toca durante 30 compases, esos 15 pentagramas ocupan espacio INÚTIL. MuseScore puede ocultarlos automáticamente.

    1. **Formato → Estilo → Pentagrama → Ocultar pentagramas vacíos dentro del sistema**.
    2. Marcar "Sí" u "Ocultar automáticamente".
    3. Configurar "No ocultar en el primer sistema" (para que el nombre del instrumento aparezca al inicio).

    !!! warning "No ocultar demasiado agresivamente"
        Si el oboe toca en el compás 1, descansa 2 compases, y vuelve en el compás 4, ocultar su pentagrama por 2 compases hace que el director "pierda" el instrumento visualmente. Regla general: ocultar SOLO si el silencio es de 4+ compases.

    ### Saltos de sistema y de página

    - **Salto de sistema** (Enter en la barra de herramientas de saltos o arrastrar desde paleta **Saltos y espaciadores**): fuerza un nuevo sistema. Usar al final de secciones musicales o cuando el sistema actual está demasiado apretado.
    - **Salto de página** (paleta **Saltos y espaciadores → Salto de página**): fuerza nueva página.
    - **Espaciador** (paleta **Saltos y espaciadores → Espaciador**): NO es un salto. Agrega espacio horizontal o vertical entre pentagramas o notas. Útil para "abrir" visualmente una partitura congestionada.

    > Insertar captura de la misma partitura ANTES y DESPUÉS de aplicar formato profesional: ocultar pentagramas vacíos, ajustar márgenes, saltos de sistema estratégicos.

???+ note "Trabajar con ensambles grandes: flujo de trabajo en MuseScore"

    ### Paso a paso para una partitura de 10+ instrumentos

    1. **Crear la partitura.**
       - **Archivo → Nuevo**.
       - Seleccionar la plantilla más cercana a tu ensamble (ej. "Orquesta" o "Banda de concierto").
       - Si no existe plantilla, elegir "Instrumentos" y agregar manualmente en el orden correcto.
       - Establecer tonalidad, compás y tempo.

    2. **Configurar el formato ANTES de escribir notas.**
       - Tamaño de página, márgenes.
       - Tamaño de pentagrama (5.0 mm para full score).
       - Configurar ocultamiento de pentagramas vacíos.
       - Agregar brackets y llaves a las familias instrumentales.
       - Verificar nombres de instrumentos (completos y abreviados).

    3. **Componer en tono de concierto.**
       - Activá el botón de tono de concierto.
       - Componé escuchando las alturas REALES.
       - Verificá rangos instrumentales.

    4. **Agregar marcas de ensayo temprano.**
       - Insertá letras de ensayo (`Ctrl + M`) en puntos estructurales: cada 8–16 compases o al inicio de cada sección nueva.
       - Las marcas de ensayo se heredan a las partes automáticamente.

    5. **Revisar la partitura general.**
       - Desactivá tono de concierto. Verificá armaduras de instrumentos transpositores.
       - Revisá que los pentagramas vacíos se oculten correctamente.
       - Agregá saltos de sistema para mejorar la distribución visual.

    6. **Generar las partes.**
       - Archivo → Partes → Generar todas.
       - **Para CADA parte individual**, revisá el checklist completo (tamaño, saltos de página, pausas multi-compás, cues, números de compás, marcas de ensayo).

    7. **Exportar.**
       - Exportar partitura general como PDF.
       - Exportar cada parte individual como PDF (Archivo → Exportar → Exportar partes...).

---

## Actividad en Classroom

### Tarea: S21 — Notación para ensambles grandes

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S21_cuarteto.mscz`, una partitura para cuarteto de cuerdas (Violín I, Violín II, Viola, Violonchelo) en Re Mayor (2 sostenidos), 4/4, 40 compases, con una pieza original completa (melodía en Vl I, acompañamiento en Vl II y Vla, bajo en Vc) pero SIN brackets, SIN marcas de ensayo, SIN ocultamiento de pentagramas vacíos, SIN partes generadas y con tamaño de pentagrama estándar (demasiado pequeño para partes individuales); (b) `ejercicio_S21_banda.mscz`, una partitura para banda de 10 instrumentos (Flauta, Oboe, Clarinete en Si♭, Saxofón alto, Saxofón tenor, Trompa en Fa, Trompeta en Si♭, Trombón, Tuba, Percusión [caja, bombo, platillos]) en Mi♭ Mayor (3 bemoles), 4/4, 56 compases, con una obra completa pero con problemas de formato: pentagramas demasiado juntos, sin ocultamiento de vacíos, brackets mal configurados (maderas y metales mezclados), saltos de página en lugares incorrectos para las partes.

1. **Cuarteto de cuerdas: formato profesional.** Abrí `ejercicio_S21_cuarteto.mscz`:
    - **Brackets y llaves**: agregá un bracket cuadrado `[` que agrupe los 4 pentagramas (familia de cuerdas). Luego, agregá una llave `{` que una el Violín I y Violín II (son la misma sub-familia). El bracket DEBE cubrir los 4 instrumentos. La llave, solo los dos violines.
    - **Tamaño de pentagrama**: reducí el tamaño a 5.5 mm para la partitura general (Formato → Estilo → Tamaño).
    - **Ocultamiento de pentagramas**: configurá el ocultamiento de pentagramas vacíos. En este cuarteto, probablemente ningún pentagrama esté vacío (es música de cámara), pero configuralo igual por práctica.
    - **Marcas de ensayo**: insertá marcas de ensayo (letras A, B, C, D...) cada 10 compases aproximadamente (compases 1, 11, 21, 31). Usá `Ctrl + M`.
    - **Saltos de sistema**: agregá saltos de sistema estratégicamente para que cada sistema tenga 4–5 compases y la página se vea balanceada.
    - Exportá la partitura general como PDF (`APELLIDO_S21_cuarteto_score.pdf`).
    - **Generar partes individuales**: Archivo → Partes → Generar todas. Para CADA parte (Vl I, Vl II, Vla, Vc):
      - Aumentá el tamaño de pentagrama a 7.5 mm.
      - Verificá los saltos de página: asegurate de que cada página termine en un lugar donde el músico pueda voltear cómodamente.
      - Verificá que las marcas de ensayo y los números de compás sean visibles.
      - Exportá CADA parte como PDF individual: `APELLIDO_S21_cuarteto_Vl1.pdf`, `APELLIDO_S21_cuarteto_Vl2.pdf`, `APELLIDO_S21_cuarteto_Vla.pdf`, `APELLIDO_S21_cuarteto_Vc.pdf`.

2. **Banda de concierto: diagnóstico y corrección.** Abrí `ejercicio_S21_banda.mscz`:
    - **Diagnóstico inicial.** Inspeccioná la partitura y anotá en un papel TODOS los problemas que encontrés antes de tocar nada. Se espera que encuentres al menos 8 problemas.
    - **Problemas a buscar y corregir:**
      - Brackets desorganizados: las maderas y los metales comparten brackets; los saxofones están agrupados con los metales en lugar de las maderas. Corregí: un bracket para maderas (Fl, Ob, Cl, Sax A, Sax T), otro para metales (Tpa, Tpt, Tbn, Tuba), otro para percusión.
      - Sin llave para la percusión: los 3 pentagramas de percusión (caja, bombo, platillos) deben estar unidos con una llave `{`.
      - Pentagramas demasiado juntos: aumentá la distancia entre pentagramas a 4.0 mm y entre sistemas a 7.0 mm.
      - Sin ocultamiento de vacíos: activá el ocultamiento de pentagramas vacíos. En esta obra de 56 compases, probablemente la percusión no toca en todos los sistemas.
      - Tamaño de pentagrama inadecuado: reducí a 5.0 mm para la partitura general.
      - Sin marcas de ensayo: insertá marcas cada 8 compases (A, B, C, D, E, F, G).
      - Nombres de instrumento ausentes o incorrectos: verificá que cada pentagrama muestre el nombre correcto en el primer sistema y su abreviatura en sistemas siguientes.
      - Saltos de página mal ubicados para las partes: al generar las partes, verificá que las páginas volteen en silencios o pausas.
    - **Documentá las correcciones**: para cada problema que encontraste y corregiste, agregá un Staff Text oculto (hacelo invisible en Propiedades) o una nota en un bloc de notas aparte explicando qué estaba mal y cómo lo arreglaste.
    - Exportá la partitura general corregida como PDF (`APELLIDO_S21_banda_score.pdf`).

3. **Generación y edición de partes de la banda.** Sobre la banda ya corregida:
    - **Generar todas las partes**: Archivo → Partes → Generar todas (10 partes).
    - **Para CADA parte individual:**
      - Tamaño de pentagrama: 7.5 mm.
      - Revisar saltos de página: usar la vista "Diseño de página" y verificar que NO haya cambios de página en medio de pasajes activos. Insertar saltos manuales si es necesario.
      - Verificar pausas multi-compás: instrumentos como la tuba o la percusión probablemente tienen silencios largos. ¿Están agrupados?
      - Agregar cues (entradas guía): para instrumentos con silencios de más de 12 compases, copiar una frase melódica de otro instrumento (en tamaño pequeño: 60–70%) para que el músico sepa cuándo entrar.
      - Verificar que las marcas de ensayo y números de compás sean visibles.
    - Exportar TODAS las 10 partes como PDFs individuales con nombres descriptivos.

4. **Creación de ensamble: partitura y partes desde cero.** Creá una NUEVA partitura: `APELLIDO_Nombre_S21_ensamble.mscz`.
    - **Ensamble**: 8 instrumentos a elección (mínimo: 2 maderas, 2 metales, 1 percusión, 2 cuerdas — o combinación equivalente). Si preferís, usá: Flauta, Clarinete en Si♭, Saxofón alto en Mi♭, Trompeta en Si♭, Trombón, Violín, Violonchelo, Piano.
    - **Tonalidad**: Sol menor (2 bemoles). Compás: 4/4. 32 compases.
    - **Formato previo**: configurá TODO antes de escribir notas:
      - Tamaño de página A4.
      - Tamaño de pentagrama: 5.5 mm (full score).
      - Brackets: maderas `[`, metales `[`, cuerdas `[`, piano con llave `{` (si incluiste piano).
      - Ocultamiento de pentagramas vacíos activado.
      - Marcas de ensayo insertadas (cada 8 compases).
    - **Componé en tono de concierto** una pieza original en Sol menor. No necesita ser una sinfonía: 32 compases con melodía, armonía, bajo y algo de percusión rítmica.
    - **Generá las 8 partes individuales** con el checklist completo.
    - **Exportá**:
      - Partitura general: `APELLIDO_Nombre_S21_ensamble_score.pdf`
      - Las 8 partes individuales como PDF.

5. **Reflexión sobre ensambles grandes.** En Classroom, respondé:
    - ¿Cuál es la diferencia más importante entre una partitura general y una parte individual, más allá del número de pentagramas? Pensá en términos de USUARIO: ¿quién lee cada una y qué necesita ver?
    - ¿Por qué es CRÍTICO que los saltos de página en las partes individuales ocurran en silencios y no en medio de pasajes activos? ¿Qué consecuencias prácticas tendría para un músico en un concierto real?
    - Describí el orden instrumental que usaste en tu ensamble propio. ¿Seguiste el orden estándar orquestal (maderas → metales → percusión → cuerdas) o lo modificaste? Justificá tu decisión.

### Entregables

- [ ] `APELLIDO_S21_cuarteto_score.pdf` (partitura general del cuarteto con brackets, marcas, saltos)
- [ ] `APELLIDO_S21_cuarteto_Vl1.pdf`, `..._Vl2.pdf`, `..._Vla.pdf`, `..._Vc.pdf` (4 partes individuales)
- [ ] `APELLIDO_S21_banda_corregida.mscz`
- [ ] `APELLIDO_S21_banda_score.pdf` (partitura general corregida)
- [ ] 10 partes individuales de la banda corregida como PDF
- [ ] `APELLIDO_Nombre_S21_ensamble.mscz`
- [ ] `APELLIDO_Nombre_S21_ensamble_score.pdf` (partitura general)
- [ ] 8 partes individuales del ensamble propio como PDF
- [ ] Documento/listado de diagnóstico con los problemas encontrados en la banda (Parte 2)
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) cuál fue el mayor desafío al preparar partes individuales y cómo lo resolviste.

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Formato del cuarteto | Brackets correctos (bracket para cuerdas + llave para violines); 5.5 mm; marcas de ensayo; saltos de sistema; pentagramas ocultos configurados | 2–3 elementos faltantes o incorrectos | Formato sin cambios significativos |
| Partes del cuarteto | 4 partes con pentagrama 7.5 mm cada una; saltos de página en silencios; marcas visibles; exportadas correctamente | 3 partes correctas | ≤2 partes correctas |
| Diagnóstico de la banda | ≥8 problemas identificados y documentados ANTES de corregir | 5–7 problemas identificados | ≤4 problemas identificados |
| Corrección de banda | Brackets reorganizados; llave de percusión; espaciado; ocultamiento; tamaño; marcas de ensayo; nombres; TODO corregido | 5–6 elementos corregidos | ≤4 elementos corregidos |
| Partes de la banda | 10 partes exportadas; todas con 7.5 mm, saltos correctos, pausas multi-compás y cues en silencios largos | 7–9 partes correctas | ≤6 partes correctas |
| Ensamble propio | 8 instrumentos; formato previo completo; composición original en Sol menor; brackets; partes generadas | Ensamble completo pero formato incompleto | Composición incompleta o sin formato |
| Reflexión | 3 respuestas con comprensión de la diferencia partitura vs. parte y justificación del orden instrumental | 2 respuestas correctas | ≤1 respuesta correcta |

---

*Basado en: MuseScore Studio 4 Handbook — Advanced topics: Parts, Staff/Part properties, Brackets and braces, Page layout concepts | https://handbook.musescore.org*
