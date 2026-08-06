# Sesión 27: Estilos, fuentes y numeración de compases

📚 Handbook → Formatting: Fonts, Measure numbers, Score properties | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="estilo-texto"></a> **Estilo de texto (Text style)** | Conjunto de propiedades tipográficas (fuente, tamaño, negrita, cursiva, alineación, color) que se aplican a un TIPO específico de texto en la partitura. MuseScore tiene estilos predefinidos para: título, subtítulo, compositor, letrista, número de compás, indicación de tempo, matiz, texto de pentagrama, y muchos más. Cambiar un estilo afecta a TODAS las instancias de ese tipo en la partitura. |
    | <a id="fuente-musical"></a> **Fuente musical (Music font)** | Tipo de letra especializado que contiene SÍMBOLOS MUSICALES en lugar de caracteres alfabéticos: cabezas de nota, claves, silencios, alteraciones, matices, articulaciones. MuseScore 4 usa **Leland** como fuente musical por defecto (creada por Muse Group, inspirada en las ediciones de Breitkopf & Härtel del siglo XIX). Otras fuentes incluyen Bravura (estilo más moderno), Gonville (estilo más redondeado), y Petaluma (estilo de música de cámara). |
    | <a id="fuente-texto"></a> **Fuente de texto (Text font)** | Tipo de letra estándar (alfabética) para los textos de la partitura: títulos, indicaciones de tempo, letra, matices en texto, números de compás. MuseScore 4 usa **Edwin** como fuente de texto por defecto (diseñada para complementar a Leland). Se puede cambiar a cualquier fuente instalada en el sistema (Times New Roman, Arial, etc.). |
    | <a id="leland"></a> **Leland (fuente musical)** | La fuente musical oficial de MuseScore 4. Su nombre es un homenaje a Leland Smith, pionero de la notación musical por computadora en Stanford. Sus glifos están dibujados para ser claros, elegantes y con un peso visual balanceado. A diferencia de fuentes musicales antiguas (que eran digitalizaciones de grabados metálicos), Leland fue DISEÑADA para pantalla. |
    | <a id="edwin"></a> **Edwin (fuente de texto)** | La fuente de texto oficial de MuseScore 4. Incluye todos los caracteres necesarios para partituras: letras estándar, caracteres con diacríticos (ü, ñ, ç, é), símbolos musicales en texto (♩, ♪, 𝄞), y números con alineación especial para compases. Está pensada para ser legible en tamaños pequeños (números de compás en particellas de orquesta). |
    | <a id="measure-number"></a> **Número de compás (Measure number)** | Numeración automática que MuseScore coloca al inicio de cada compás (o cada N compases, según la configuración). Es EL sistema de referencia universal en ensayos: "vamos del compás 47" significa que todos los músicos encuentran el compás marcado como 47 en su parte. Sin números de compás, un ensayo de orquesta es un caos logístico. |
    | <a id="intervalo-medida"></a> **Intervalo de numeración** | Frecuencia con la que aparece el número de compás. Por defecto, MuseScore muestra el número en el PRIMER compás de cada sistema. En particellas de orquesta, típicamente se numera cada 1, 5 o 10 compases para que el músico pueda ubicarse rápidamente. Se configura en **Formato → Estilo → Números de compás**. |
    | <a id="score-properties"></a> **Propiedades de la partitura (Score properties)** | Metadatos de la obra: título, subtítulo, compositor, letrista, copyright, año de creación, número de catálogo, editor, dedicatoria. Estos datos NO solo son informativos: se usan para generar automáticamente la cabecera de la primera página, las páginas de título, y los metadatos de exportación (PDF, MusicXML, MP3). Se editan en **Archivo → Propiedades de la partitura**. |
    | <a id="style-profile"></a> **Perfil de estilo (Style profile)** | Conjunto completo de TODAS las configuraciones de formato de una partitura (fuentes, tamaños, distancias, alineaciones, visibilidad de elementos) guardado como un archivo .mss (MuseScore Style). Permite aplicar el MISMO estilo de formato a múltiples partituras. Ej: "Quiero que todas mis partituras de coro usen fuente Petaluma, A5 horizontal, márgenes de 10 mm, y números de compás cada 5 compases." |
    | <a id="cabecera-pie"></a> **Cabecera y pie de página (Header / Footer)** | Texto que aparece en la parte superior (cabecera) o inferior (pie) de cada página de la partitura o de las particellas. Suele contener: nombre de la obra, compositor, número de página o nombre del instrumento (en particellas). Se configura en **Formato → Estilo → Cabecera, pie de página**. |
    | <a id="copyright-metadata"></a> **Copyright y metadatos** | Información legal y de catalogación de la obra. El copyright protege los derechos del compositor. En el contexto académico, incluir copyright en tus partituras establece tu autoría públicamente. Aunque tu obra no esté registrada formalmente, el copyright "© [año] [nombre]" declara tu propiedad intelectual. |
    | <a id="alineacion-texto"></a> **Alineación de texto** | Posición horizontal y vertical de un elemento textual respecto al pentagrama o al compás. Un título suele estar centrado. Un número de compás suele estar alineado a la izquierda del compás. Una indicación de tempo suele estar alineada a la izquierda sobre el pentagrama. Una mala alineación es un marcador instantáneo de partitura amateur. |

???+ note "La tipografía de la partitura: fuentes musicales y de texto"

    La tipografía es el 50% de la personalidad visual de una partitura. Dos partituras con las MISMAS notas pero con DIFERENTES fuentes se ven como obras completamente distintas. Elegir las fuentes correctas es una decisión EDITORIAL, no técnica.

    ### El dúo Leland + Edwin

    MuseScore 4 viene con una combinación tipográfica diseñada específicamente para notación musical:

    | Fuente | Tipo | ¿Qué dibuja? | Personalidad |
    |---|---|---|---|
    | **Leland** | Musical | Notas, claves, silencios, alteraciones, matices, articulaciones | Clásica, elegante, atemporal. Inspirada en los grabados alemanes del siglo XIX (Breitkopf & Härtel). |
    | **Edwin** | Texto | Títulos, indicaciones de tempo, letra, números de compás, texto de pentagrama | Sobria, funcional, altamente legible. Diseñada para NO llamar la atención y dejar que la música hable. |

    ### Otras fuentes musicales disponibles

    | Fuente | Estilo | ¿Para qué tipo de música? |
    |---|---|---|
    | **Bravura** | Moderna, nítida, ligeramente angulosa | Música contemporánea, partituras de estudio, ediciones académicas. Es la fuente de referencia del estándar SMuFL (Standard Music Font Layout). |
    | **Gonville** | Redondeada, cálida, más "manuscrita" | Música de cámara, coral, jazz. Recuerda a las partituras copiadas a mano de mediados del siglo XX. |
    | **Petaluma** | Compacta, limpia, optimizada para pentagramas pequeños | Partituras de orquesta y banda donde el espacio es crítico. Menor peso visual por nota. |
    | **MuseJazz** | Estilo manuscrito de jazz (cabezas de nota inclinadas, plicas más gruesas) | Partituras de jazz, big band, música popular. Fuente de texto complementaria: MuseJazzText. |

    ### Cómo cambiar las fuentes

    1. **Fuente musical**: **Formato → Estilo → Partitura → Fuente musical**. Seleccionar Leland, Bravura, Gonville, Petaluma o MuseJazz.
    2. **Fuente de texto**: **Formato → Estilo → Estilos de texto → [elemento]**. Por ejemplo, para cambiar la fuente del título: **Estilos de texto → Título → Fuente → Edwin (u otra)**.
    3. **Tamaños de fuente**: cada estilo de texto tiene su propio tamaño. Los títulos suelen ser más grandes (24–30 pt), las indicaciones de tempo intermedias (12–14 pt), los números de compás pequeños (8–10 pt).

    !!! warning "No mezcles fuentes musicales sin criterio"
        Cambiar la fuente musical a MITAD de la partitura es como escribir un párrafo con 3 tipografías distintas: un desastre visual. Elegí UNA fuente musical para toda la partitura. La coherencia tipográfica es un pilar del diseño editorial profesional. Si querés experimentar, hacelo en copias separadas.


???+ note "Numeración de compases: el GPS del ensayo"

    Los números de compás son el sistema de navegación más importante de una partitura de ensamble. Sin ellos, el director no puede decir "vamos del 47". Sin ellos, los músicos no pueden marcar sus partes. Sin ellos, un ensayo se convierte en: "empecemos donde dice 'Allegro'... no, más adelante... donde el oboe hace esa nota larga...".

    ### Configuración básica

    **Formato → Estilo → Números de compás:**

    | Parámetro | Qué hace | Valor típico |
    |---|---|---|
    | **Intervalo** | Cada cuántos compases aparece el número | 1 (cada compás), 5 o 10 (particellas de orquesta) |
    | **Primer compás numerado** | A partir de qué compás empieza la numeración | 1 (por defecto) |
    | **Mostrar en el primer compás del sistema** | Siempre visible al inicio de cada sistema | Activado (SIEMPRE — es crucial para la orientación) |
    | **Posición horizontal** | Alineación respecto al compás | Izquierda (estándar) |
    | **Posición vertical** | Distancia sobre/bajo el pentagrama | Sobre el pentagrama, 2–3 sp de distancia |
    | **Fuente y tamaño** | Tipografía específica para números de compás | Edwin, 8–10 pt |

    ### Numeración en particellas vs. partitura completa

    | Contexto | Intervalo recomendado | Justificación |
    |---|---|---|
    | **Partitura completa (conductor)** | Cada 1 compás, o cada 5 si la página es densa | El director necesita precisión absoluta |
    | **Particella de orquesta** | Cada 5 o 10 compases | El músico solo necesita orientación general; cada compás sobrecargaría la página |
    | **Particella de cámara** | Cada 1 compás | Con pocos músicos, la precisión es importante y el espacio no es problema |
    | **Particella con muchos silencios** | Cada compás durante los silencios multicompás, cada 5-10 durante pasajes activos | El músico que está contando 47 compases de silencio AGRADECE los números |
    | **Estudio / ejercicio** | Cada 1 compás | Facilita la referencia del profesor ("compás 12, la tercera corchea") |

    ### Numeración especial

    - **Reiniciar numeración**: con un salto de sección. El primer compás después del salto vuelve a ser "1". Útil para movimientos separados.
    - **Excluir compás de la numeración**: útil para compases de anacrusa (el compás incompleto del inicio NO debería contarse como "1").
    - **Números en recuadro o círculo**: para ensayos. Algunos formatos (especialmente teatro musical y bandas sonoras) usan números en recuadro o círculo en lugar de números simples, para máxima visibilidad en condiciones de poca luz (foso de orquesta).

    !!! danger "El número de compás NUNCA debe ser invisible"
        Si los números de compás no se ven, el ensayo se detiene cada 2 minutos para que los músicos pregunten "¿en qué compás estamos?". El tiempo del director es CARO. No le hagas perder el tiempo por no configurar bien los números de compás.


???+ note "Propiedades de la partitura: la identidad de la obra"

    Las propiedades de la partitura son el DNI de tu obra. Una partitura sin metadatos es una obra ANÓNIMA. Si alguien encuentra tu PDF dentro de 10 años, ¿va a saber quién la escribió?

    ### Metadatos esenciales

    **Archivo → Propiedades de la partitura:**

    | Campo | Ejemplo | ¿Dónde aparece? |
    |---|---|---|
    | **Título** | Sonata para violín y piano en Sol menor | Primera página (cabecera), metadatos del PDF, exportación MusicXML |
    | **Subtítulo** | I. Allegro con brio | Debajo del título, primera página |
    | **Compositor** | Juan Pérez (1998– ) | Primera página (lado derecho), metadatos |
    | **Letrista** | (si aplica) | Primera página (lado izquierdo) |
    | **Copyright** | © 2026 Juan Pérez. Todos los derechos reservados. | Primera página (pie), metadatos del PDF |
    | **Número de catálogo** | Op. 14, No. 2 | Junto al título (ediciones académicas) |
    | **Dedicatoria** | A mi madre | Página de título (si existe) |
    | **Año de composición** | 2026 | Metadatos, página de título |

    ### El triángulo de la primera página

    Toda partitura profesional responde TRES preguntas en su primera página:

    ```
    ┌────────────────────────────────────────────┐
    │                                              │
    │            Título de la obra                  │
    │            Subtítulo (si hay)                 │
    │                                              │
    │  Compositor                    Letrista      │
    │  (derecha)                     (izquierda)    │
    │                                              │
    │  ═══════════ [música] ════════════════════   │
    │                                              │
    │  © año compositor. Todos los derechos...     │
    │  (pie de página, centrado o izquierda)       │
    └────────────────────────────────────────────┘
    ```

    **Título** (arriba, centrado): ¿QUÉ es esta obra?  
    **Compositor** (derecha): ¿QUIÉN la escribió?  
    **Copyright** (pie): ¿A QUIÉN pertenece legalmente?

    ### Cabecera y pie de página

    En **Formato → Estilo → Cabecera, pie de página** podés configurar texto que aparece en CADA página:

    - **Cabecera**: típicamente el título de la obra (páginas pares) o el compositor (páginas impares).
    - **Pie**: número de página, copyright, o nombre del instrumento (en particellas).

    **Particellas**:
    - Cabecera: nombre del instrumento (ej. "Violín I") + título de la obra.
    - Pie: número de página.
    - Esto asegura que si las hojas se mezclan (y SIEMPRE se mezclan en los ensayos), cada músico sepa exactamente qué hoja corresponde a qué parte.

    !!! tip "Metadatos en la exportación"
        Cuando exportás un PDF desde MuseScore, los campos de Título, Compositor y Copyright se incrustan en los metadatos del archivo PDF. Esto significa que si alguien busca "Sonata en Sol menor" en su computadora, tu PDF va a aparecer en los resultados. Si dejás los metadatos vacíos, tu PDF es un fantasma digital: existe pero es imposible de encontrar.


???+ note "Perfiles de estilo: tu identidad editorial"

    Un perfil de estilo es como una "plantilla de formato". Configurás TODO una vez (fuentes, tamaños, distancias, numeración, cabeceras, etc.) y lo aplicás a todas tus partituras con un solo clic.

    ### ¿Por qué usar perfiles de estilo?

    - **Consistencia**: todas tus partituras se ven como parte de una misma "colección". Un pianista que lee 3 obras tuyas seguidas siente que pertenecen al mismo compositor.
    - **Eficiencia**: en lugar de configurar fuentes y formatos CADA VEZ que empezás una partitura nueva, cargás tu perfil y empezás a escribir inmediatamente.
    - **Profesionalismo**: los compositores y editores serios tienen su propio estilo editorial. Es su "marca visual".

    ### Cómo crear y cargar un perfil de estilo

    **Guardar un perfil**:
    1. Formatear una partitura exactamente como querés que se vean TODAS tus obras futuras.
    2. **Formato → Guardar estilo...**.
    3. Elegir ubicación y nombre (ej. `mi_estilo_coral.mss`, `estilo_orquesta.mss`).
    4. El archivo .mss contiene TODAS las configuraciones de formato.

    **Cargar un perfil**:
    1. Abrir la partitura nueva (sin formato).
    2. **Formato → Cargar estilo...**.
    3. Seleccionar el archivo .mss guardado.
    4. La partitura nueva adopta inmediatamente TODO el formato del perfil.

    ### Qué incluye un perfil de estilo

    - Fuentes musical y de texto.
    - Tamaños y estilos de todos los tipos de texto (título, compositor, tempo, matices, números de compás, etc.).
    - Configuración de página (tamaño de papel, márgenes, escala).
    - Distancias entre pentagramas, sistemas y otros elementos verticales.
    - Numeración de compases (intervalo, posición, fuente).
    - Cabecera y pie de página.
    - Estilos de líneas, barras de compás, plicas y otros elementos gráficos.
    - Prácticamente TODO lo que no son las notas mismas.

    !!! tip "Creá perfiles para cada tipo de ensamble"
        Un perfil para música de cámara (A4 vertical, fuente Leland, márgenes generosos). Otro para orquesta (A3/Tabloide horizontal, fuente Petaluma, pentagramas compactos). Otro para coro (A5, fuente Gonville, letra más grande). Otro para ejercicios de clase (A4 vertical, números de compás visibles, márgenes amplios para anotaciones del profesor). Cada tipo de partitura tiene necesidades de formato distintas. No uses el mismo perfil para todo.


---

## Actividad en Classroom

### Tarea: S27 — Estilos, fuentes y numeración de compases

> **Material necesario**: el docente proporcionará dos archivos: (a) `ejercicio_S27_sin_identidad.mscz`, una partitura de ensamble (cuarteto de saxofones: soprano, alto, tenor, barítono) de 40 compases SIN metadatos, con fuentes por defecto, numeración de compases insuficiente y sin cabecera/pie de página; (b) `ejercicio_S27_perfil.mscz`, una partitura de coro (SATB: soprano, alto, tenor, bajo) de 28 compases con texto, lista para ser estilizada con un perfil editorial.

1. **Restauración de identidad editorial.** Abrí `ejercicio_S27_sin_identidad.mscz`:
    - Esta partitura de cuarteto de saxofones está "desnuda": buena música, PERO sin título, sin compositor, sin copyright, sin números de compás adecuados, sin cabecera ni pie de página. Es una obra anónima esperando ser identificada.
    - **Paso 1 — Metadatos**: completá **Archivo → Propiedades de la partitura** con:
        - Título: inventá uno apropiado para un cuarteto de saxofones.
        - Subtítulo (opcional): un indicador de tempo o carácter (ej. "Andante espressivo").
        - Compositor: TU nombre.
        - Copyright: "© [año actual] [tu nombre]. Todos los derechos reservados."
    - **Paso 2 — Primera página**: verificá que el título, compositor y copyright aparezcan correctamente en la primera página. Ajustá el tamaño y alineación si es necesario.
    - **Paso 3 — Numeración de compases**: configurá los números de compás para que:
        - Aparezcan en CADA compás (intervalo = 1).
        - Sean visibles en el primer compás de cada sistema.
        - Tengan un tamaño legible (al menos 9 pt).
        - Aparezcan SOBRE cada pentagrama individual (no solo en el primer pentagrama del sistema).
    - **Paso 4 — Cabecera y pie de página**: configurá para que en cada página aparezca:
        - Cabecera: título de la obra (página par) / compositor (página impar).
        - Pie: número de página centrado + "© [año] [tu nombre]" a la izquierda.
    - **Paso 5 — Fuentes**: experimentá cambiando la fuente musical de Leland a Bravura y a Gonville. Probá cómo se ve la partitura con cada una. Elegí la que más te guste y justificá tu elección en Classroom.
    - Guardá como `APELLIDO_Nombre_S27_identidad.mscz`.

2. **Diseño de perfil editorial para coro.** Abrí `ejercicio_S27_perfil.mscz`:
    - Esta partitura de coro SATB con texto debe ser estilizada para verse como una edición coral profesional.
    - **Configurá**:
        - Fuente musical: **Gonville** (es la más adecuada para música coral, por su calidez y legibilidad en pentagramas con letra).
        - Fuente de texto: mantené Edwin para títulos, pero asegurate de que la letra de la obra use un tamaño suficiente (≥ 11 pt) para que un coreuta de 60 años pueda leerla sin lentes.
        - Tamaño de papel: A5 horizontal (típico de ediciones corales de bolsillo).
        - Márgenes: 10 mm en todos los lados (formato compacto).
        - Numeración de compases: cada 5 compases (suficiente para coro, sin sobrecargar).
        - Cabecera: nombre de la cuerda (Soprano, Alto, Tenor, Bajo) en CADA página.
        - Pie: número de página centrado.
    - **Ajustes finales**:
        - Asegurate de que la letra esté correctamente alineada con las notas.
        - Verificá que los matices y respiraciones (comas) no se superpongan con la letra.
        - Si hay sílabas largas (melismas), verificá que la línea de extensión sea visible.
    - Guardá como `APELLIDO_Nombre_S27_coral.mscz`.
    - Guardá el perfil de estilo como `APELLIDO_Nombre_S27_perfil_coral.mss` (**Formato → Guardar estilo**).
    - Exportá el PDF: `APELLIDO_Nombre_S27_coral.pdf`.

3. **Comparación tipográfica.** Abrí nuevamente `ejercicio_S27_sin_identidad.mscz` (la versión original sin modificar) y cambiale SOLO la fuente musical. Creá 3 versiones rápidas:
    - `APELLIDO_Nombre_S27_leland.pdf` (Leland, la original)
    - `APELLIDO_Nombre_S27_bravura.pdf` (Bravura)
    - `APELLIDO_Nombre_S27_gonville.pdf` (Gonville)
    - En Classroom, publicá una comparación visual de las 3 fuentes (captura de los primeros 2 sistemas de cada una, lado a lado) y respondé: ¿qué fuente preferís para este cuarteto de saxofones? ¿Por qué? ¿Cambiaría tu elección si fuera una partitura de orquesta sinfónica?

4. **Reflexión.** En Classroom, respondé:
    - ¿Qué diferencia hace tener metadatos completos en una partitura? ¿Por qué creés que tantas partituras en internet (MuseScore.com, IMSLP amateur) NO tienen copyright ni metadatos?
    - Después de esta sesión, ¿vas a incluir copyright en TODAS tus partituras? ¿Por qué sí o por qué no?
    - ¿Qué aprendiste sobre el impacto de las fuentes en la percepción de una partitura? ¿Creés que el músico promedio nota la diferencia entre Leland y Bravura o es un detalle "para obsesivos"?

### Entregables

- [ ] `APELLIDO_Nombre_S27_identidad.mscz`
- [ ] `APELLIDO_Nombre_S27_coral.mscz`
- [ ] `APELLIDO_Nombre_S27_perfil_coral.mss`
- [ ] `APELLIDO_Nombre_S27_coral.pdf`
- [ ] `APELLIDO_Nombre_S27_leland.pdf`
- [ ] `APELLIDO_Nombre_S27_bravura.pdf`
- [ ] `APELLIDO_Nombre_S27_gonville.pdf`
- [ ] Comentario en Classroom con: (a) justificación de elección de fuente para el cuarteto, (b) comparación tipográfica lado a lado, (c) respuestas a las 3 preguntas de reflexión

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Metadatos | Título, compositor, copyright completos y correctamente visibles en la primera página | Faltan 1–2 campos | ≥3 campos ausentes |
| Numeración de compases | Intervalo 1, visibles en cada pentagrama, primer compás de sistema, tamaño legible | Configuración correcta pero tamaño pequeño o visibilidad parcial | Sin numeración o intervalo inadecuado |
| Cabecera y pie | Cabecera con título/compositor según paridad; pie con página + copyright | Configuración incompleta (falta cabecera o pie) | Sin cabecera ni pie |
| Perfil coral | Fuente Gonville, A5 horizontal, márgenes compactos, letra legible, cabecera con nombre de cuerda; perfil .mss guardado | Mayoría de parámetros correctos pero falta algún ajuste clave | Formato sin cambios significativos |
| Comparación tipográfica | 3 PDFs exportados; comparación visual publicada; justificación argumentada | 2 fuentes comparadas | Sin comparación |
| Reflexión | 3 respuestas con análisis de metadatos, copyright y percepción tipográfica | 2 respuestas correctas | ≤1 respuesta |

---

*Basado en: MuseScore Studio 4 Handbook — Formatting: Fonts, Measure numbers, Score properties | https://handbook.musescore.org*
