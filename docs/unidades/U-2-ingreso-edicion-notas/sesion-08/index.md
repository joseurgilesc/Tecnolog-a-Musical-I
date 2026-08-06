# Sesión 8: Valores irregulares, puntillos y agrupación rítmica

📚 Handbook → Notation: Rhythm, meter & measures — Tuplets, Beams; Basics: Entering notes and rests (dots); Notation: Grace notes | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="valor-irregular"></a> **Valor irregular / Grupillo (tuplet)** | Grupo de notas que divide una duración en un número de partes que no es potencia de 2 y que, por lo tanto, no se puede escribir con figuras convencionales. Ejemplo: un tresillo de corcheas ocupa el espacio de una negra (3 notas donde normalmente entrarían 2). |
    | <a id="tresillo"></a> **Tresillo (triplet)** | El valor irregular más común: tres notas en el espacio de dos del mismo valor. Se indica con un `3` sobre o bajo el grupo. |
    | <a id="quintillo"></a> **Quintillo (quintuplet)** | Cinco notas en el espacio de cuatro del mismo valor. Se indica con un `5`. |
    | <a id="seisillo"></a> **Seisillo / Sextillo (sextuplet)** | Seis notas en el espacio de cuatro del mismo valor. Se indica con un `6`. |
    | <a id="puntillo"></a> **Puntillo (dot)** | Punto que, colocado a la derecha de una figura o silencio, aumenta su duración en la mitad de su valor. Se ingresa con la tecla `.` antes de escribir la nota. |
    | <a id="doble-puntillo"></a> **Doble puntillo** | Dos puntos que añaden la mitad más la mitad de la mitad de la duración original (3/4 adicionales). Disponible en la paleta o en el panel de propiedades. |
    | <a id="barra-agrupacion"></a> **Barra de agrupación (beam)** | Línea horizontal que conecta figuras de corchea o más cortas para agruparlas visualmente según la métrica. MuseScore las genera automáticamente según las propiedades del compás. |
    | <a id="barrado"></a> **Barrado (beaming)** | Patrón de agrupación de corcheas, semicorcheas y fusas mediante barras. Se puede modificar manualmente nota por nota o mediante la configuración del compás. |
    | <a id="nota-adorno"></a> **Nota de adorno (grace note)** | Nota pequeña que se escribe antes de una nota principal y no cuenta en la duración total del compás. Puede ser una apoyatura (con barra) o una acciaccatura (sin barra, tachada). |

???+ note "Valores irregulares: tresillos, quintillos y más"

    Un valor irregular (tuplet) divide una duración en un número de partes iguales que no son potencia de 2. Es una de las herramientas más expresivas de la notación rítmica.

    ### Crear un tresillo simple

    El tresillo de corcheas (3 corcheas donde normalmente entrarían 2) es el caso más común:

    1. Seleccionar o navegar hasta la nota o silencio donde querés que comience el tresillo.
    2. Elegir la **duración total** del tresillo. Para un tresillo de corcheas que ocupa una negra, presionar `5` (negra).
    3. Presionar `Ctrl + 3` (`Cmd + 3` en macOS).
    4. Ingresar las notas del tresillo.

    La secuencia completa: `N` → `5` → `Ctrl + 3` → ingresar tres notas.

    > Insertar captura de la creación de un tresillo: el cursor azul sobre el pentagrama, el indicador `3` apareciendo sobre el grupo de tres corcheas recién ingresadas.

    ### Atajos para valores irregulares

    | Divisiones | Atajo |
    |---|---|
    | Duillo (2 en espacio de 3) | `Ctrl + 2` |
    | Tresillo | `Ctrl + 3` |
    | Cuatrillo (4 en espacio de 3) | `Ctrl + 4` |
    | Quintillo | `Ctrl + 5` |
    | Seisillo / Sextillo | `Ctrl + 6` |
    | Septillo | `Ctrl + 7` |
    | Octillo | `Ctrl + 8` |
    | Novenillo | `Ctrl + 9` |

    Todos funcionan con el mismo principio: primero elegís la duración base, después el atajo, después ingresás las notas.

    ### Valores irregulares anidados

    Es posible crear un tresillo dentro de otro tresillo (o cualquier combinación anidada):

    1. Crear el tresillo exterior normalmente (ej. `5` → `Ctrl + 3`).
    2. Seleccionar una nota **dentro** del tresillo.
    3. Crear el tresillo interior (ej. `4` → `Ctrl + 3`).

    > Insertar captura de tresillos anidados: un tresillo de corcheas donde una de las corcheas es a su vez otro tresillo de semicorcheas.

    ### Crear un valor irregular personalizado

    Para valores que no están en los atajos (ej. 11:8, 13:4):

    1. Seleccionar la posición inicial.
    2. Elegir la duración total del grupo.
    3. Ir a **Añadir → Grupos irregulares → Otro...** (o clic prolongado en el icono de tresillo → Otro...).
    4. En el diálogo, definir:
       - **Relación**: cuántas notas en el espacio de cuántas (ej. 11 en espacio de 8).
       - **Formato de número**: mostrar el número (`11`), la relación (`11:8`) o ninguno.
       - **Corchete**: automático, siempre visible o nunca.

    ### Propiedades del valor irregular

    Seleccionando el número del tresillo, en el panel **Propiedades** se puede ajustar:
    - **Dirección**: arriba o abajo del pentagrama.
    - **Tipo de número**: solo el número (`3`), la relación (`3:2`), o sin número.
    - **Tipo de corchete**: automático, con corchete, o sin corchete.

    ### Repetir valores irregulares en serie

    Cuando necesitás varios tresillos seguidos:
    1. Crear el primer tresillo.
    2. Seleccionar el tresillo completo (rango).
    3. Presionar `R`. Cada pulsación crea un nuevo tresillo justo a continuación.

    !!! tip "El orden correcto: duración primero, división después"
        El error más común es presionar `Ctrl + 3` antes de seleccionar la duración. Si lo hacés al revés, MuseScore no sabe en qué espacio debe repartir las 3 notas. Siempre: **duración → atajo → notas**.

???+ note "Puntillo simple y doble"

    El puntillo es una de las herramientas rítmicas más usadas y también una de las que más errores genera por mala comprensión de su efecto matemático.

    ### ¿Cuánto agrega un puntillo?

    | Figura original | Con puntillo | Equivalencia |
    |---|---|---|
    | Blanca (2 tiempos) | Blanca con puntillo (3 tiempos) | Blanca + negra |
    | Negra (1 tiempo) | Negra con puntillo (1.5 tiempos) | Negra + corchea |
    | Corchea (½ tiempo) | Corchea con puntillo (¾ tiempo) | Corchea + semicorchea |
    | Semicorchea (¼ tiempo) | Semicorchea con puntillo (⅜ tiempo) | Semicorchea + fusa |

    La regla es siempre la misma: **el puntillo añade la mitad del valor de la figura a la que acompaña**.

    ### Ingresar una nota con puntillo

    En modo de ingreso (`N`):
    1. Seleccionar la duración (`4` para corchea, `5` para negra, etc.).
    2. Presionar `.` (punto).
    3. Ingresar la nota.

    Ejemplo para una negra con puntillo: `N` → `5` → `.` → `C`.

    ### Doble puntillo

    Agrega la mitad más la mitad de la mitad (3/4 adicionales). Una negra con doble puntillo equivale a negra + corchea + semicorchea. No tiene un atajo directo de teclado; se aplica desde:
    - La paleta **Puntillos** (en Más → Figuras).
    - El panel **Propiedades**, en la sección **Nota**, activando "Doble puntillo".

    ### Puntillo en silencios

    Funciona exactamente igual: `N` → `5` → `.` → `0` produce un silencio de negra con puntillo.

    !!! warning "El puntillo no es un adorno"
        No subestimes el puntillo. Un puntillo mal colocado desbalancea todo el compás. Antes de guardar, seleccioná cada compás y contá mentalmente cuánto suman sus figuras: si no cierra, algún puntillo está mal ubicado.

???+ note "Agrupación rítmica: barras de corcheas y semicorcheas"

    Las barras que unen corcheas, semicorcheas y fusas no son decorativas: son una herramienta de **legibilidad métrica**. Un barrado correcto comunica al intérprete dónde está cada pulso.

    ### Barrado automático por compás

    MuseScore agrupa automáticamente las figuras según las reglas del compás. Por ejemplo, en 4/4, las corcheas se agrupan por pulsos (2+2+2+2), y en 6/8 se agrupan en dos bloques de 3.

    ### Cambiar el barrado predeterminado de un compás

    Para modificar cómo se agrupan todas las notas de un compás a nivel global:

    1. Seleccionar la indicación de compás.
    2. En el panel **Propiedades**, clic en **Propiedades de indicación de compás**.
    3. En **Grupos de barras**, hacer clic en las figuras del diagrama para activar o desactivar la unión de barras en cada pulso.
    4. Clic en **Aceptar**.

    Esto afecta a TODAS las notas de ese compás en toda la partitura.

    ### Modificar el barrado de notas individuales

    Para cambiar el barrado de una nota concreta sin afectar al resto:

    1. Seleccionar la nota.
    2. Ir a la pestaña **Barra** en la sección **Nota** del panel **Propiedades**.

    Las opciones disponibles, de izquierda a derecha:

    | Icono | Efecto |
    |---|---|
    | Auto | Restablece el barrado por defecto del compás |
    | Sin barra | Rompe TODAS las barras que entran o salen de la nota |
    | Romper barra izquierda | Rompe solo la barra que llega a la nota desde la izquierda |
    | Romper barras internas (8) | Deja solo una barra (para semicorcheas que pasarían a verse como corcheas) |
    | Romper barras internas (16) | Deja solo dos barras |
    | Unir barras | Fuerza la unión con la nota anterior |

    ### Barras sobre silencios

    Para extender una barra a través de un silencio:
    1. Seleccionar el silencio.
    2. Aplicar **Unir barras** o **Romper barra izquierda** según corresponda.

    ### Barras sobre líneas divisorias

    Para extender una barra a través de una barra de compás:
    1. Seleccionar la primera nota después de la barra divisoria.
    2. Aplicar **Unir barras**.

    ### Barras en disminución/aumento (feathered beams)

    Para indicar accelerando o ritardando gráficamente, MuseScore permite barras que se abren en abanico. Seleccionar la barra y en el panel **Propiedades** elegir **Acelerar** o **Desacelerar**. Nota: esto es solo visual; no afecta la reproducción.

    > Insertar captura comparativa: un mismo pasaje rítmico con barrado convencional (por pulsos) y con barrado personalizado (unión entre pulsos), mostrando el panel de propiedades de barra.

???+ note "Notas de adorno: apoyaturas y acciaccaturas"

    Las notas de adorno son notas pequeñas que preceden a una nota principal y no ocupan tiempo propio en el compás (su duración se toma de la nota que adornan).

    ### Tipos de notas de adorno

    | Tipo | Visualmente | Efecto en reproducción |
    |---|---|---|
    | **Apoyatura (appoggiatura)** | Nota pequeña sin tachar; sin barra | Toma la mitad de la duración de la nota principal (si es binaria) o 2/3 (si es ternaria) |
    | **Acciaccatura** | Nota pequeña con barra oblicua tachándola | No toma tiempo medible; suena muy breve, casi simultánea con la principal |

    ### Insertar una nota de adorno

    1. Seleccionar la nota principal (la que va a ser adornada).
    2. Ir a la paleta **Notas de adorno** (Grace notes).
    3. Elegir **Apoyatura** o **Acciaccatura**.
    4. Ingresar la altura de la nota de adorno con el teclado (`A`–`G`).

    También podés agregar varias notas de adorno consecutivas antes de una misma nota principal. Cada una se ingresa después de la anterior.

    ### Propiedades de las notas de adorno

    Seleccionando una nota de adorno, en el panel **Propiedades** podés ajustar:
    - Si se muestra la plica y la barra.
    - Su posición (arriba o abajo).

    > Insertar captura de una apoyatura y una acciaccatura antes de una negra, con los dos tipos visibles lado a lado.

---

## Actividad en Classroom

### Tarea: S08 — Valores irregulares y agrupación rítmica

> **Material necesario**: el docente proporcionará el archivo `ejercicio_S08_ritmo.mscz` con una partitura para instrumento de teclado (piano) en Do mayor, 4/4, 24 compases con una base rítmica y melódica simple. Los compases 1 a 12 contienen ritmo básico con corcheas y semicorcheas; los compases 13 a 24 están vacíos.

1. **Tresillos en diferentes figuras.** En los compases 1 a 4, reemplazá grupos de corcheas por tresillos de corchea (`5` → `Ctrl + 3`). Construí al menos:
    - Dos compases con tresillos de corcheas.
    - Un compás con un tresillo de negras (blanca como duración base: `6` → `Ctrl + 3`).
    - Verificá que cada compás siga sumando 4 tiempos exactos.

2. **Quintillo y sextillo.** En los compases 5 a 8:
    - Construí un quintillo de semicorcheas sobre una negra (`5` → `Ctrl + 5`). Ingresá 5 notas que quepan en el espacio de 1 tiempo.
    - Construí un sextillo de semicorcheas sobre una negra (`5` → `Ctrl + 6`).
    - Compará visual y auditivamente: ¿cuál suena más rápido? ¿Por qué?

3. **Valor irregular anidado.** En el compás 9, creá un tresillo exterior de corcheas. Dentro de la primera corchea de ese tresillo, insertá otro tresillo de semicorcheas. El resultado debe ser: tres corcheas en espacio de una negra, y la primera de esas corcheas está subdividida en tres semicorcheas.

4. **Puntillos y dobles puntillos.** En los compases 11 y 12:
    - Ingresá un patrón rítmico que combine negras con puntillo (`.`) y corcheas.
    - Ingresá al menos una nota con **doble puntillo** (usando la paleta de puntillos o el panel de propiedades).
    - Verificá que cada compás cuadre: sumá mentalmente las duraciones.

5. **Agrupación personalizada.** En los compases 13 a 20, creá tu propia melodía de 8 compases en 4/4 que incluya abundantes corcheas y semicorcheas. Luego:
    - Modificá el barrado de al menos 3 compases para que las corcheas se agrupen distinto al patrón por defecto. Experimentá con **Unir barras** y **Romper barra izquierda**.
    - Hacé que una barra atraviese un silencio (barrado sobre silencio).
    - Probá el barrado sobre la barra divisoria entre dos compases (barra que cruza la línea divisoria).

6. **Notas de adorno.** En los compases 21 a 24:
    - Insertá 4 notas de adorno en diferentes lugares: al menos 2 apoyaturas y 2 acciaccaturas.
    - Reproducí el pasaje con y sin las notas de adorno. ¿Se nota la diferencia auditiva entre apoyatura y acciaccatura?

7. **Escucha crítica.** Reproducí la partitura completa y escuchá con atención:
    - ¿Los tresillos suenan uniformes (cada nota dura exactamente lo mismo)?
    - ¿Los compases con puntillos están equilibrados?
    - ¿La agrupación de barras ayuda a leer el ritmo o lo dificulta?
    - Corregí cualquier error rítmico que detectes.

### Entregables

- [ ] `APELLIDO_Nombre_S08_ritmo_v01.mscz` (partitura con todos los ejercicios rítmicos)
- [ ] `APELLIDO_Nombre_S08_ritmo_v01.pdf`
- [ ] Captura de pantalla del tresillo anidado (compás 9) con el panel de propiedades visible
- [ ] Captura de pantalla de un compás con barrado personalizado (antes/después o el panel de propiedades de barra)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Tresillos | Todos los tresillos suman correctamente (no sobra ni falta tiempo en los compases) y están bien construidos | 1–2 compases con error de duración | ≥3 compases con tresillos incorrectos |
| Quintillo y sextillo | Ambos están correctamente construidos; la comparación auditiva evidencia la diferencia de velocidad | Uno correcto, otro incorrecto | No realizó quintillo o sextillo |
| Tresillo anidado | El tresillo exterior y el interior son correctos; el compás suma exactamente 4 tiempos | Anidamiento presente pero con error de duración | No tiene tresillo anidado o está mal construido |
| Puntillos | Las notas con puntillo y doble puntillo están correctas; cada compás cuadra rítmicamente | Puntillos correctos pero el doble puntillo no se usó | Compases con error rítmico por mal uso del puntillo |
| Agrupación personalizada | Barrado modificado en ≥3 compases; barra sobre silencio presente; el resultado es legible | Barrado modificado pero sin barra sobre silencio o poco legible | No modificó el barrado |
| Notas de adorno | Dos apoyaturas y dos acciaccaturas correctamente insertadas; diferencias auditivas identificadas | Un tipo presente, otro ausente | No insertó notas de adorno |
| Escucha crítica | Revisó y corrigió errores rítmicos detectados auditivamente | Escuchó pero no corrigió | No reprodujo ni revisó |

---

*Basado en: MuseScore Studio 4 Handbook — Tuplets, Beams; MuseScore 3 Handbook — Notation: Tuplets, Beams, Grace notes | https://handbook.musescore.org*
