# Sesión 14: Texto, letra y cifrado

📚 Handbook → Text: Lyrics, Chord notation systems, Staff Text, Rehearsal marks | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="letra"></a> **Letra (lyrics)** | Texto cantado que se alinea sílaba a sílaba con las notas de una melodía. En MuseScore, cada sílaba se ingresa debajo de su nota correspondiente y se navega con `Barra espaciadora`. La letra se separa en sílabas con guiones y las sílabas sostenidas se indican con un guion bajo (`_`) de melisma. |
    | <a id="guion-silabico"></a> **Guion silábico (syllabic hyphen)** | Guion ` - ` que se coloca entre dos sílabas de una misma palabra cuando éstas se distribuyen en notas diferentes. Ejemplo: "ca-`-`mi-`-`no" — cada sílaba en una nota distinta. |
    | <a id="melisma"></a> **Melisma** | Cuando una sola sílaba se sostiene a lo largo de varias notas. Se indica con un guion bajo `_` por cada nota adicional que la sílaba abarque. Ejemplo: "A-`_`-`_`-mén" — la sílaba "A" se canta durante tres notas. |
    | <a id="cifrado-armonico"></a> **Cifrado armónico (chord symbol)** | Notación abreviada que indica la armonía sobre el pentagrama. Usa letras mayúsculas para el acorde base (C = Do mayor, Am = La menor), números para extensiones (C7, Cmaj7), alteraciones para el bajo (C/E = Do mayor con Mi en el bajo) y símbolos especiales para cualidades (Cm, Cº, Cø). Va colocado sobre el pentagrama, típicamente sobre la melodía o el acompañamiento. |
    | <a id="cifrado-funcional"></a> **Cifrado funcional (Roman numeral analysis)** | Sistema de análisis armónico que usa números romanos para indicar la función de cada acorde respecto a la tonalidad (I, IV, V, vi). Complementa al cifrado armónico con información teórica. En MuseScore, se ingresa como texto de pentagrama o usando herramientas de análisis específicas. |
    | <a id="texto-pentagrama"></a> **Texto de pentagrama (staff text)** | Texto libre que se coloca sobre o debajo del pentagrama y se aplica a ese pentagrama específicamente. Se usa para indicaciones de interpretación: *pizz.*, *arco*, *con sord.*, *solo*, *tutti*, cambios de carácter (*dolce*, *espressivo*). Atajo: `Ctrl + T` (`Cmd + T` en macOS). |
    | <a id="texto-sistema"></a> **Texto de sistema (system text)** | Similar al texto de pentagrama pero se aplica a TODOS los pentagramas del sistema simultáneamente. Se usa para indicaciones globales: tempo, carácter general, referencias de sección. Atajo: `Ctrl + Shift + T` (`Cmd + Shift + T`). |
    | <a id="marca-ensayo"></a> **Marca de ensayo (rehearsal mark)** | Letra mayúscula o número en un recuadro que marca puntos de referencia en la partitura para facilitar los ensayos ("vamos desde la letra D"). MuseScore las genera automáticamente en secuencia A, B, C... pero se pueden personalizar. Atajo: `Ctrl + M` (`Cmd + M`). |
    | <a id="bajo-cifrado"></a> **Bajo alterado / slash chord** | En cifrado armónico, cuando el bajo no es la fundamental del acorde se indica con una barra: C/E significa "acorde de Do mayor con Mi en el bajo". También se usa para bajos cromáticos (C/E♭, C/D) y walkings de bajo que no cambian la armonía. |
    | <a id="extenso-voz"></a> **Texto de extensión a una voz (lyrics verse)** | MuseScore permite múltiples líneas de letra. La línea 1 (verso 1) va asociada por defecto. Líneas adicionales (verso 2, 3) se pueden agregar para partituras corales con varias estrofas. Se accede desde **Añadir → Texto → Letra** y seleccionando el número de verso. |
    | <a id="alineacion-letra"></a> **Alineación de letra** | La sílaba de la letra se alinea automáticamente con la cabeza de su nota correspondiente. Si una sílaba abarca un melisma (varias notas), los guiones bajos `_` se extienden hasta la última nota del melisma y MuseScore dibuja una línea de extensión automáticamente. |

???+ note "Letra alineada a melodía: ingreso sílaba a sílaba"

    Escribir letra en MuseScore es ingresar sílabas que se "pegan" a las notas. El programa se encarga de la alineación, los guiones entre sílabas y las líneas de melisma.

    ### Activar el modo de ingreso de letra

    1. Seleccionar la primera nota que lleva texto.
    2. Presionar `Ctrl + L` (`Cmd + L` en macOS). Aparece un cursor de texto debajo de la nota.
    3. Escribir la primera sílaba y presionar `Space` (barra espaciadora) para avanzar a la siguiente nota.
    4. Continuar sílaba → `Space` → sílaba → `Space`...

    ### Separación silábica con guiones

    Cuando una palabra se divide en sílabas sobre diferentes notas:

    ```
    Nota 1: "co-"   ← el guion va PEGADO a la sílaba
    Nota 2: "ra-"   ← MuseScore agrega el guion entre notas automáticamente
    Nota 3: "zón"
    ```

    Al escribir, ingresás:
    ```
    co- [Space] ra- [Space] zón [Space]
    ```

    !!! tip "El guion va pegado a la sílaba, no separado"
        Escribí `co-` (guion pegado). NO escribas `co -` (guion con espacios). Si dejás espacio, MuseScore interpreta que hay dos sílabas diferentes y la separación se rompe.

    ### Melismas: una sílaba, varias notas

    Cuando una sílaba se sostiene sobre MÚLTIPLES notas (melisma), usás el guion bajo `_`:

    ```
    Nota 1: "A"     ← la sílaba empieza acá
    Nota 2: "_"     ← guion bajo = la sílaba sigue sonando
    Nota 3: "_"     ← guion bajo = sigue sonando
    Nota 4: "mén"   ← termina la sílaba, empieza la siguiente
    ```

    Al escribir, ingresás:
    ```
    A [Space] _ [Space] _ [Space] mén [Space]
    ```

    MuseScore dibuja automáticamente una línea horizontal de extensión desde la sílaba "A" hasta la última nota del melisma.


    ### Navegación rápida al ingresar letra

    | Tecla | Acción |
    |---|---|
    | `Space` | Avanzar a la nota siguiente |
    | `Shift + Space` | Avanzar a la nota siguiente saltando un melisma (avanza hasta la última nota del melisma) |
    | `Ctrl + Space` (`Cmd + Space`) | Insertar un espacio en blanco dentro de la letra (para palabras compuestas o respiraciones en el texto) |
    | `-` (guion) | Insertar guion para separación silábica |
    | `_` (guion bajo) | Marcar continuación de melisma (sílaba sostenida) |
    | `←` / `→` | Moverse entre sílabas ya escritas para corregir |

    ### Varios versos (estrofas)

    Para canciones con múltiples estrofas:
    1. Escribir el verso 1 normalmente.
    2. Seleccionar la primera nota del pentagrama.
    3. Ir a **Añadir → Texto → Letra** y seleccionar **Verso 2** (o el número que corresponda).
    4. Ingresar el texto del segundo verso de la misma manera (sílaba + `Space`).

    Cada verso queda en su propia línea, perfectamente alineado con las notas. MuseScore maneja hasta 10 versos simultáneos.

    !!! warning "No uses el guion bajo para otra cosa"
        En el ingreso de letra, el guion bajo `_` tiene un significado MUY específico: melisma. Si escribís `_` donde debería ir una sílaba real, MuseScore lo interpretará como continuación de la sílaba anterior, no como texto. Para escribir un guion bajo literal (como parte del texto), usá el panel de edición de texto y no el modo de ingreso de letra.

???+ note "Cifrado armónico: acordes sobre el pentagrama"

    El cifrado armónico es la notación estándar para indicar armonía en jazz, pop, música popular y hojas de ruta (*lead sheets*). Se coloca sobre el pentagrama, típicamente alineado con los tiempos fuertes del compás.

    ### Activar el ingreso de cifrado

    1. Seleccionar la nota donde empieza el acorde.
    2. Presionar `Ctrl + K` (`Cmd + K` en macOS).
    3. Escribir el cifrado del acorde. Ejemplos: `C`, `Am`, `F#m7`, `Bb7`, `Dm7b5`.
    4. Presionar `Space` para avanzar a la siguiente nota/tiempo.

    ### Notación estándar de cifrado

    | Elemento | Ejemplo | Significado |
    |---|---|---|
    | **Fundamental** | `C` | Do mayor (tríada) |
    | **Menor** | `Cm`, `C-`, `c` | Do menor (la `m` es lo más estándar en MuseScore) |
    | **Séptima dominante** | `C7` | Do mayor con séptima menor |
    | **Séptima mayor** | `Cmaj7`, `CΔ` | Do mayor con séptima mayor |
    | **Séptima menor** | `Cm7`, `C-7` | Do menor con séptima menor |
    | **Semidisminuido** | `Cm7b5`, `Cø` | Do menor séptima con quinta bemol |
    | **Disminuido** | `Cº`, `Cdim` | Do disminuido |
    | **Aumentado** | `C+`, `Caug` | Do aumentado |
    | **Suspenso** | `Csus4`, `Csus2` | Do con cuarta o segunda suspendida |
    | **Bajo alterado** | `C/E` | Do mayor con Mi en el bajo |

    ### Atajos de alteraciones en cifrado

    Durante el ingreso de cifrado (`Ctrl + K`):
    - `b` (letra be minúscula) se convierte automáticamente en ♭ (bemol).
    - `#` se mantiene como sostenido.
    - Podés escribir `bb` para doble bemol y `x` o `##` para doble sostenido.

    ### Cifrado y reproducción

    MuseScore NO reproduce los acordes basándose solo en el cifrado. El cifrado armónico es información para el intérprete humano. Si querés que MuseScore reproduzca la armonía, necesitás escribir las notas reales en el pentagrama o usar plugins de acompañamiento automático.

    !!! tip "Cifrado vs. escritura de acordes"
        El cifrado armónico y los acordes escritos en el pentagrama son dos cosas distintas. El cifrado (`Ctrl + K`) es texto sobre el pentagrama que lee el intérprete. Las notas del acorde son sonidos reales que escribe el compositor. En una *lead sheet* profesional, la melodía está escrita en notas y la armonía está en cifrado sobre el pentagrama. No se duplica la información: no escribas las notas del acorde si ya pusiste el cifrado, a menos que tengas una razón específica.


???+ note "Texto de pentagrama y texto de sistema"

    Además de la letra y el cifrado, MuseScore permite insertar texto libre con diferentes alcances.

    ### Texto de pentagrama (Staff Text) — `Ctrl + T`

    Se aplica a UN solo pentagrama. Usos típicos:
    - Instrucciones técnicas: *pizz.* (pizzicato), *arco*, *con sordino*, *senza sordino*.
    - Indicaciones de carácter: *dolce*, *espressivo*, *cantabile*, *marcato*.
    - Cambios de interpretación: *solo*, *tutti*, *divisi*, *unis*.

    **Insertar:**
    1. Seleccionar la nota o compás donde va el texto.
    2. Presionar `Ctrl + T`.
    3. Escribir el texto y hacer clic fuera para confirmar.

    ### Texto de sistema (System Text) — `Ctrl + Shift + T`

    Se aplica a TODOS los pentagramas del sistema. Usos típicos:
    - Indicaciones de tempo: *Allegro*, *Andante*, *rit.*, *accel.*.
    - Cambios de carácter globales: *più mosso*, *meno mosso*.
    - Referencias estructurales: *Tempo I*, *Come prima*.

    **Insertar:**
    1. Seleccionar la nota o compás.
    2. Presionar `Ctrl + Shift + T`.
    3. Escribir el texto y clic fuera.

    !!! warning "No confundir Staff Text con System Text"
        Si ponés *pizz.* como System Text, TODOS los instrumentos intentarán tocar pizzicato, incluido el piano o la flauta (lo cual no tiene sentido). El Staff Text es por pentagrama. El System Text es global. Elegí el correcto según a quién va dirigida la instrucción.

    ### Editar propiedades del texto

    Seleccionando cualquier texto insertado, el panel **Propiedades** ofrece:
    - **Fuente, tamaño, estilo** (negrita, cursiva).
    - **Alineación** respecto a la nota.
    - **Posición** (arriba/abajo del pentagrama).
    - **Color** (útil para edición, no se imprime por defecto).


???+ note "Marcas de ensayo: navegación para el director"

    Las marcas de ensayo son letras o números en un recuadro que permiten al director decir "vamos desde la letra D" sin tener que contar compases. Son esenciales en partituras de orquesta, banda y ensambles grandes.

    ### Insertar una marca de ensayo

    1. Seleccionar el compás o la barra donde va la marca.
    2. Presionar `Ctrl + M` (`Cmd + M`).
    3. MuseScore inserta automáticamente la siguiente letra en secuencia: A, B, C, D...

    ### Personalizar la marca

    Por defecto, MuseScore usa letras mayúsculas (A, B, C...). Para cambiar:
    1. Seleccionar la marca de ensayo.
    2. En el panel **Propiedades**, editar el texto.
    3. Podés usar números (1, 2, 3...), combinaciones (A1, B2...), o texto libre.

    ### Convenciones

    - **Letras mayúsculas** (A, B, C...) → lo más común en orquestas y bandas.
    - **Números de compás en recuadro** → común en partituras de estudio y música contemporánea (ej. `[42]`).
    - **Números de sección** → en musicales y ópera (1, 2, 3... o A1, A2...).

    ### Marcas de ensayo y saltos de navegación

    Las marcas de ensayo NO afectan la reproducción ni los saltos de navegación. Son puramente una ayuda visual para el ensayo. No las confundas con segnos, Codas o repeticiones: las marcas de ensayo no producen saltos en la ejecución.


    !!! tip "No pongas marcas de ensayo en cada compás"
        Las marcas de ensayo deben colocarse en puntos estructurales: inicio de sección, cambio de tempo, entrada de solista, pasaje difícil. Si ponés una marca cada 2 compases, pierden su utilidad. La frecuencia típica es cada 8–16 compases o en cada cambio de sección.

---

## Actividad en Classroom

### Tarea: S14 — Texto, letra y cifrado

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S14_letra.mscz`, una melodía para voz en Do mayor, 4/4, 12 compases SIN letra pero con el texto de la canción en un recuadro de texto al inicio; (b) `ejercicio_S14_cifrado.mscz`, una partitura para piano (melodía en pentagrama superior, acompañamiento simple en inferior) en Sol mayor, 4/4, 16 compases con la melodía escrita pero SIN cifrado armónico; (c) `ejercicio_S14_ensayo.mscz`, una partitura para orquesta de cuerdas (violín I, violín II, viola, violonchelo) en Re mayor, 3/4, 32 compases con secciones claramente diferenciadas pero SIN marcas de ensayo y SIN indicaciones de interpretación (*pizz.*, *arco*, etc.).

1. **Ingreso de letra en la melodía vocal.** Abrí `ejercicio_S14_letra.mscz`:
    - Leé el texto completo de la canción en el recuadro.
    - Activá el modo de ingreso de letra (`Ctrl + L`) sobre la primera nota.
    - Ingresá sílaba por sílaba, usando `Space` para avanzar.
    - Asegurate de usar **guiones silábicos** (`-`) entre sílabas de una misma palabra: `can-` [Space] `ción`.
    - Identificá dónde hay **melismas** (sílabas que abarcan más de una nota) y usá guiones bajos `_` para las notas adicionales del melisma.
    - Verificá que cada sílaba esté alineada con su nota correspondiente. Si una sílaba quedó en la nota equivocada, seleccionala y arrastrala, o borrala y reingresala.
    - Reproducí la melodía: ¿la letra se "lee" fluidamente siguiendo las notas?

2. **Cifrado armónico sobre el piano.** Abrí `ejercicio_S14_cifrado.mscz`:
    - Escuchá la melodía y el acompañamiento. Identificá los cambios armónicos (escuchá cuándo "cambia el color" del acompañamiento).
    - Activá el ingreso de cifrado (`Ctrl + K`) sobre la primera nota de cada cambio armónico.
    - Ingresá el cifrado correspondiente: acordes mayores con letra mayúscula (`G`, `C`, `D`), menores con `m` (`Am`, `Em`, `Bm`), séptimas donde corresponda (`D7`, `G7`).
    - Si hay acordes con bajo alterado (el bajo no toca la fundamental), indicalo: `G/B`, `C/E`, `D/F#`.
    - Reproducí y verificá que los cambios de cifrado coincidan con los cambios armónicos reales.
    - **Desafío**: si identificás un acorde disminuido o semidisminuido, escribilo con la notación correcta (`º` o `m7b5`).

3. **Texto de interpretación en la orquesta de cuerdas.** Abrí `ejercicio_S14_ensayo.mscz`:
    - Insertá **marcas de ensayo** (`Ctrl + M`) al inicio de cada sección claramente diferenciada (debe haber al menos 4 secciones: A, B, C, D o las que identifiques). Usá letras mayúsculas en secuencia.
    - Insertá **texto de pentagrama** (`Ctrl + T`) en los instrumentos de cuerda donde corresponda:
      - *pizz.* al inicio de un pasaje en pizzicato (identificalo por la articulación o el carácter).
      - *arco* cuando el pasaje en pizzicato termina.
      - *dolce* o *espressivo* en pasajes líricos.
      - *solo* donde un instrumento tenga una línea melódica destacada.
    - Insertá **texto de sistema** (`Ctrl + Shift + T`) para indicar:
      - El tempo al inicio de la partitura: *Moderato*.
      - Cualquier cambio de tempo que detectes (*più mosso*, *rit.*).
    - Revisá: ¿cada texto de pentagrama está en el instrumento correcto? ¿Los textos de sistema aparecen en todos los pentagramas?

4. **Integración: lead sheet completa.** En el mismo archivo `ejercicio_S14_cifrado.mscz` ya editado:
    - Copiá la melodía del pentagrama superior (mano derecha) a un NUEVO pentagrama de voz solista. Andá a **Añadir → Instrumentos**, agregá "Voice" o "Soprano", copiá la melodía y eliminá el pentagrama superior del piano (o silencialo).
    - Ahora tenés una estructura de *lead sheet*: melodía en la voz + acompañamiento en el piano.
    - Agregá la letra de una canción conocida que encaje con la melodía (o inventá una breve). Ingresala con `Ctrl + L` sobre la voz solista.
    - Verificá que el cifrado armónico siga visible sobre la melodía.
    - Agregá marcas de ensayo cada 4 u 8 compases.
    - Exportá como PDF. ¿El resultado se parece a una *lead sheet* profesional?

5. **Reflexión sobre texto en la partitura.** En Classroom, respondé:
    - ¿Qué diferencia hay entre Staff Text y System Text? Da un ejemplo concreto de cuándo usarías cada uno en una partitura de orquesta.
    - ¿Por qué el cifrado armónico no se reproduce en MuseScore? ¿Cuál es su propósito entonces?
    - ¿En qué se diferencia un melisma de una separación silábica normal? ¿Cómo se indica cada uno en el ingreso de letra de MuseScore?

### Entregables

- [ ] `APELLIDO_Nombre_S14_letra_v01.mscz` (melodía vocal con letra completa)
- [ ] `APELLIDO_Nombre_S14_letra_v01.pdf`
- [ ] `APELLIDO_Nombre_S14_cifrado_v01.mscz` (piano con cifrado armónico + versión lead sheet)
- [ ] `APELLIDO_Nombre_S14_cifrado_v01.pdf`
- [ ] `APELLIDO_Nombre_S14_ensayo_v01.mscz` (orquesta con marcas de ensayo y textos de interpretación)
- [ ] `APELLIDO_Nombre_S14_ensayo_v01.pdf`
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) breve explicación de las decisiones que tomaste para el cifrado armónico (¿cómo identificaste los cambios de armonía?)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Ingreso de letra | Todas las sílabas alineadas; guiones silábicos correctos; melismas con `_`; sin sílabas huérfanas | Letra ingresada pero con 2–3 errores de alineación o guiones mal colocados | Letra incompleta o con >3 errores |
| Cifrado armónico | Cifrado correcto en ≥80% de los cambios; variedad de tipos (M, m, 7, bajo alterado); coincidencia auditiva con la armonía | Cifrado presente pero con 3–4 errores de análisis armónico | Cifrado ausente o incorrecto en >50% |
| Marcas de ensayo | ≥4 marcas en secciones estructurales; secuencia lógica (A, B, C, D); visibles en todos los pentagramas | 2–3 marcas o colocación no estructural | ≤1 marca |
| Texto de interpretación | ≥4 Staff Texts correctamente asignados a instrumentos específicos; ≥2 System Texts globales; sin confusiones | Textos presentes pero con 1–2 asignaciones incorrectas (Staff ↔ System) | Textos ausentes o mal asignados sistemáticamente |
| Lead sheet integrada | Melodía + letra + cifrado + marcas de ensayo; formato coherente y legible | Lead sheet creada pero falta algún elemento | No se entregó la lead sheet |
| Reflexión | Responde las 3 preguntas con ejemplos concretos; demuestra comprensión de los conceptos | Responde 2 de 3 correctamente o sin ejemplos | No responde o las respuestas son incorrectas |

---

*Basado en: MuseScore Studio 4 Handbook — Lyrics, Chord notation systems, Staff Text, Rehearsal marks | https://handbook.musescore.org*
