# Sesión 22: Configuración y uso de teclado MIDI

📚 Handbook → Basics: Note input modes (MIDI keyboard), Preferences | Herramientas: MuseScore Studio 4, teclado MIDI (físico o virtual), Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="midi"></a> **MIDI (Musical Instrument Digital Interface)** | Protocolo estándar de comunicación entre instrumentos musicales electrónicos, computadoras y software. No transmite audio (sonido), sino INSTRUCCIONES: qué nota se tocó, con qué velocidad, cuándo se soltó, qué pedal se pisó. Es el "lenguaje universal" de la música digital desde 1983. Un archivo MIDI pesa kilobytes; un archivo de audio (WAV, MP3) pesa megabytes. |
    | <a id="midi-keyboard"></a> **Teclado MIDI / controlador MIDI** | Dispositivo con teclas estilo piano que envía mensajes MIDI al software. NO produce sonido por sí mismo (no tiene parlantes ni generador de audio): necesita que el software (MuseScore, un DAW, un sintetizador virtual) interprete los mensajes y genere el audio. Puede tener 25, 49, 61 u 88 teclas y puede incluir ruedas de pitch bend, modulación, pads y sliders. |
    | <a id="velocity"></a> **Velocity (velocidad)** | Valor MIDI (0–127) que indica con qué fuerza se golpeó la tecla. 0 = silencio, 127 = máxima fuerza. En MuseScore, la velocity se traduce en dinámica (una nota con velocity alta suena más fuerte). Es uno de los parámetros más importantes para que una interpretación MIDI suene "humana" y no robótica. |
    | <a id="step-time"></a> **Ingreso por paso (step-time input)** | Método de ingreso de notas donde primero se selecciona la DURACIÓN (negra, corchea, etc.) y luego se indica la ALTURA (con el mouse, teclado de computadora o teclado MIDI). No importa el ritmo con que toques: MuseScore coloca la nota en la posición del cursor y avanza automáticamente. Es el método por defecto en MuseScore. |
    | <a id="real-time"></a> **Ingreso en tiempo real (real-time input)** | Método donde tocás las notas en el teclado MIDI al ritmo de la música y MuseScore las transcribe automáticamente. Requiere tocar con precisión rítmica (como si grabaras). Existen dos modos: automático (MuseScore decide las duraciones) y manual (vos indicás la duración mientras tocás). |
    | <a id="midi-channel"></a> **Canal MIDI** | "Carril" de comunicación independiente dentro de una conexión MIDI. El estándar MIDI permite 16 canales simultáneos. En MuseScore, cada instrumento del ensamble puede asignarse a un canal diferente para que los mensajes de un pentagrama no interfieran con los de otro. |
    | <a id="latency"></a> **Latencia (latency)** | Retraso entre el momento en que presionás una tecla y el momento en que escuchás el sonido. En sistemas MIDI, una latencia alta (> 20 ms) hace que tocar sea incómodo porque el sonido "llega tarde". Se reduce usando drivers ASIO (Windows), CoreAudio (Mac, nativo y sin configuración), o ajustando el tamaño del buffer de audio. |
    | <a id="pitch-bend"></a> **Pitch bend** | Mensaje MIDI que modifica la afinación de una nota hacia arriba o abajo de forma continua. Se controla con una rueda física en el teclado MIDI. En MuseScore, NO se usa el pitch bend durante el ingreso de notas: el programa espera alturas exactas del pentagrama. El pitch bend se usa en DAWs (Ableton, Logic, etc.) para efectos expresivos. |
    | <a id="quantization"></a> **Cuantización (quantization)** | Proceso de ajustar automáticamente la posición rítmica de las notas tocadas en tiempo real para que coincidan con la grilla métrica. Si tocaste una corchea "un poco adelantada", la cuantización la mueve a la posición exacta de la corchea. Es fundamental en el ingreso en tiempo real, pero un exceso de cuantización produce un resultado robótico y sin expresividad. |
    | <a id="cc-midi"></a> **Control Change (CC)** | Mensajes MIDI que transmiten cambios en parámetros del sonido: CC7 = volumen, CC10 = panorama (izquierda/derecha), CC64 = pedal de sustain, CC1 = modulación. En MuseScore, muchas marcas de expresión (dinámicas, reguladores, texto de staff) se traducen internamente en mensajes CC para la reproducción. |
    | <a id="buffer"></a> **Buffer de audio** | Memoria temporal donde el software acumula muestras de audio antes de enviarlas a la placa de sonido. Un buffer pequeño (64–128 samples) = baja latencia pero riesgo de cortes. Un buffer grande (512–1024 samples) = estable pero alta latencia. La configuración del buffer se hace en las preferencias de audio de MuseScore. |
    | <a id="midi-mapping"></a> **Mapeo MIDI (MIDI mapping)** | Asignación que define qué tecla del teclado MIDI corresponde a qué acción en MuseScore. Por defecto, las teclas blancas y negras corresponden a las notas musicales estándar. Pero MuseScore también permite mapear teclas a funciones: iniciar/detener reproducción, cambiar de compás, insertar silencios, etc. Se configura desde **Editar → Preferencias → MIDI → Accesos directos MIDI**. |

???+ note "¿Qué es MIDI y por qué importa?"

    MIDI es el sistema nervioso de la música digital. Sin MIDI, cada programa musical hablaría su propio idioma y sería imposible conectar un teclado Yamaha con una computadora Dell corriendo MuseScore.

    ### MIDI NO es audio

    Este es el error conceptual más común y más grave. Repetilo hasta que te quede grabado:

    | Característica | MIDI | Audio (WAV, MP3) |
    |---|---|---|
    | ¿Qué transmite? | Instrucciones: "tocá Do₄ con velocity 100 durante 0.5 segundos" | Forma de onda: presión del aire 44,100 veces por segundo |
    | Tamaño de archivo | Kilobytes (una sinfonía MIDI completa < 100 KB) | Megabytes (una canción en MP3 ~ 5 MB) |
    | ¿Se puede editar nota por nota? | Sí, cada nota es un evento independiente | No (sin herramientas especializadas como Melodyne) |
    | ¿Suena igual en todas las computadoras? | NO: depende del sintetizador que lo reproduzca | Sí (aproximadamente): la forma de onda es siempre igual |
    | ¿Puedo cambiar el tempo sin cambiar la afinación? | Sí: el tempo es independiente de las notas | NO: acelerar el audio cambia la afinación (efecto "chipmunk") |

    **Analogía**: MIDI es una PARTITURA digital. El audio es una GRABACIÓN. La partitura te dice qué tocar; la grabación es el sonido resultante. Podés cambiar la instrumentación de una partitura (de violín a flauta) sin reescribir nada. No podés hacer eso con una grabación.

    ### La revolución silenciosa de 1983

    Antes de MIDI, cada fabricante (Roland, Yamaha, Korg, Moog) usaba su propio protocolo. Un sintetizador Roland no se podía conectar con uno Yamaha. En 1983, los ingenieros de Sequential Circuits, Roland, Yamaha y Korg se reunieron y definieron un estándar común: MIDI 1.0. Ese estándar, con modificaciones menores, sigue vigente HOY. Es uno de los estándares más longevos y exitosos de la historia de la tecnología.

    !!! tip "El cable MIDI físico"
        El conector MIDI tradicional es un DIN de 5 pines (circular, grande). Hoy en día, la mayoría de teclados MIDI se conectan por USB. El protocolo MIDI puede viajar por cable MIDI tradicional, por USB, por Bluetooth (MIDI over BLE), o por red (MIDI over Ethernet / RTP-MIDI). Lo importante es el PROTOCOLO, no el cable.

???+ note "Configuración del teclado MIDI en MuseScore"

    Conectar un teclado MIDI a MuseScore requiere DOS pasos: conexión física y configuración en el software. Si falla uno, el teclado no funciona.

    ### Paso 1: Conexión física

    | Tipo de conexión | Cable necesario | Ventaja | Desventaja |
    |---|---|---|---|
    | **USB** (la más común) | Cable USB-A a USB-B (el cuadrado que viene con impresoras y teclados MIDI) | Plug and play, alimenta el teclado | Latencia variable, ocupa un puerto USB |
    | **MIDI DIN (5 pines)** | Cable MIDI + interfaz MIDI-USB | Conexión profesional, menor latencia | Necesita interfaz externa |
    | **Bluetooth MIDI** | No necesita cable | Sin cables, libertad de movimiento | Latencia impredecible, no recomendado para ingreso en tiempo real |

    **Procedimiento para USB**:
    1. Conectar el cable USB al teclado y a la computadora.
    2. Encender el teclado (si tiene switch de encendido).
    3. Esperar a que el sistema operativo lo reconozca (5–10 segundos).

    En Mac: el teclado aparece automáticamente en **Configuración de Audio MIDI** (`/Aplicaciones/Utilidades/Configuración de Audio MIDI.app`). En Windows: aparece en el Administrador de dispositivos como "Dispositivo de audio USB" o con el nombre del fabricante.

    ### Paso 2: Configuración en MuseScore

    1. Abrir MuseScore Studio 4.
    2. Ir a **Editar → Preferencias** (Mac: `Cmd + ,` / Windows: `Ctrl + ,`).
    3. Seleccionar la pestaña **Audio y MIDI**.
    4. En la sección **Dispositivos MIDI**, buscar el teclado en la lista **Entrada MIDI**.
    5. Si el teclado aparece, seleccionarlo como **dispositivo activo**.
    6. El teclado debería aparecer como **"Habilitado"** (indicador verde en versiones recientes).

    !!! warning "¿Mi teclado no aparece en la lista?"
        Causas comunes:
        - El teclado no está encendido (verificá el switch de power).
        - El cable USB está dañado o no hace buen contacto (probá otro cable).
        - El teclado necesita drivers (algunos modelos Roland/Korg requieren instalación de driver en Windows; en Mac generalmente no).
        - MuseScore se abrió ANTES de conectar el teclado. Solución: cerrar MuseScore, conectar el teclado, reabrir MuseScore.
        - El puerto USB no entrega suficiente energía. Probar en otro puerto o con un hub USB alimentado.

    ### Paso 3: Prueba de funcionamiento

    1. Crear una partitura nueva (cualquier plantilla).
    2. Activar el modo de ingreso de notas (`N`).
    3. Tocar una tecla en el teclado MIDI.
    4. Si la nota aparece en el pentagrama y se escucha → el teclado funciona correctamente.
    5. Si no aparece → volver a verificar los pasos anteriores.


???+ note "Modos de ingreso con teclado MIDI"

    Una vez conectado el teclado, tenés TRES formas principales de ingresar notas. Cada una sirve para situaciones diferentes.

    ### Modo 1: Ingreso por paso (Step-time) — El más usado

    **Cómo funciona**: primero elegís la duración, luego tocás la nota.

    1. Activar ingreso de notas: `N`.
    2. Seleccionar duración: clic en el ícono de negra (o atajo numérico: `5` = negra, `4` = corchea, `6` = blanca, `7` = redonda).
    3. Tocar la nota deseada en el teclado MIDI.
    4. La nota aparece en el pentagrama en la posición del cursor. El cursor avanza al siguiente pulso automáticamente.
    5. Para acordes: mantener presionadas las teclas simultáneamente. MuseScore apilará las notas en el mismo tiempo.

    **Ventajas**:
    - Precisión absoluta: cada nota va exactamente donde querés.
    - Ideal para música compleja rítmicamente (tresillos, síncopas, notas con puntillo).
    - No necesitás tocar al tempo correcto; podés tomarte tu tiempo entre nota y nota.
    - Funciona incluso si no sabés tocar piano "de verdad" (solo necesitás saber qué tecla corresponde a cada nota).

    **Desventaja**: más lento que el ingreso en tiempo real para música simple y repetitiva.

    **Atajos clave para productividad**:
    - `R`: repetir la última nota/cifra ingresada.
    - `Q`: reducir a la mitad la duración seleccionada (negra → corchea).
    - `W`: duplicar la duración (negra → blanca).
    - `Shift + W`: agregar puntillo a la duración actual.
    - `.` (punto): convertir en nota con puntillo después de ingresarla.
    - `T`: agregar ligadura de prolongación a la nota recién ingresada.

    !!! tip "Ingreso de acordes por paso"
        Para ingresar un acorde de 3 notas con teclado MIDI en step-time:
        1. Seleccionar la duración (ej. `5` para negra).
        2. Tocar simultáneamente Do + Mi + Sol en el teclado.
        3. MuseScore coloca las tres notas apiladas en el mismo pulso.
        Si querés agregar notas una por una al acorde: mantené `Shift` mientras tocás cada nota adicional.

    ### Modo 2: Ingreso en tiempo real automático — Para los que tocan piano

    **Cómo funciona**: tocás al ritmo de un metrónomo y MuseScore transcribe.

    1. Colocar el cursor en el compás donde querés empezar.
    2. Activar **Editar → Preferencias → MIDI → Modo de entrada en tiempo real** o usar el ícono de la barra de herramientas de reproducción (el botón de "grabar" rojo en la barra de transporte en algunas versiones).
    3. Configurar el tempo (con el control deslizante de tempo en la barra de transporte).
    4. MuseScore hace una cuenta regresiva (1 compás de clics de metrónomo) y empieza a grabar.
    5. Tocá junto con el metrónomo. MuseScore transcribe las notas y duraciones automáticamente.
    6. Presionar `Espacio` para detener la grabación.

    **Parámetros importantes**:
    - **Cuantización**: define la duración mínima que MuseScore va a reconocer. Si configurás "corchea", las notas más rápidas que una corchea no se transcribirán correctamente.
    - **Velocidad de entrada**: el tempo del metrónomo en BPM (pulsos por minuto).

    **Ventajas**:
    - Rapidísimo para música que podés tocar fluidamente.
    - Captura la expresividad (velocity) de tu interpretación.
    - Ideal para melodías simples, escalas, arpegios.

    **Desventajas**:
    - Requiere tocar con precisión rítmica. Si tocás "fuera de tiempo", MuseScore produce un desastre.
    - La cuantización puede malinterpretar ritmos complejos (síncopas, tresillos).
    - No funciona bien si no tenés práctica de tocar con metrónomo.

    ### Modo 3: Ingreso en tiempo real manual — Híbrido

    **Cómo funciona**: tocás las notas al tempo pero VOS decidís las duraciones.

    1. Activar el modo de ingreso (`N`).
    2. Seleccionar la duración deseada (`5` para negra, `4` para corchea).
    3. Tocar una tecla en el teclado MIDI en el momento rítmico correcto (MuseScore está reproduciendo el metrónomo).
    4. La nota se inserta con la duración que elegiste, no la que tocaste.

    **Ventaja**: combinás la velocidad del ingreso rítmico con el control de las duraciones.


    ### Comparación rápida

    | Modo | ¿Necesito tocar al tempo? | Precisión rítmica | Velocidad | Ideal para... |
    |---|---|---|---|---|
    | **Step-time** | No | Perfecta | Media | Música compleja, edición de detalles |
    | **Real-time automático** | Sí | Depende de tu precisión tocando | Alta | Melodías simples, transcripción rápida |
    | **Real-time manual** | Sí | Alta (vos elegís la duración) | Media-alta | Música con ritmo variado |

???+ note "Más allá del ingreso: el teclado MIDI como herramienta"

    El teclado MIDI no solo sirve para ingresar notas. Con los atajos MIDI, se convierte en un centro de control para MuseScore que acelera drásticamente el flujo de trabajo.

    ### Atajos MIDI: controlá MuseScore desde el teclado

    MuseScore permite asignar teclas del teclado MIDI a funciones del programa:

    | Función | Atajo sugerido (tecla MIDI) |
    |---|---|
    | **Iniciar / Detener reproducción** | La nota más grave del teclado (normalmente no usada para ingreso) |
    | **Ir al compás anterior / siguiente** | Dos teclas adyacentes en el extremo grave |
    | **Activar / Desactivar ingreso de notas** | Un botón de transporte si el teclado tiene |
    | **Insertar silencio** | Una tecla negra específica fuera del ámbito normal |

    **Cómo configurar**: **Editar → Preferencias → MIDI → Accesos directos MIDI**. Cada atajo se configura presionando la tecla MIDI deseada mientras el campo de asignación está activo.

    ### Reproducción con teclado MIDI

    Si tu teclado MIDI tiene GENERADOR DE SONIDO interno (sintetizador, no solo controlador), podés usarlo para reproducir la partitura en lugar de los sonidos por defecto de MuseScore:
    1. Ir a **Editar → Preferencias → Audio y MIDI → Salida MIDI**.
    2. Seleccionar el teclado como dispositivo de salida.
    3. Ahora la reproducción de MuseScore enviará mensajes MIDI al teclado, que generará el audio con sus propios sonidos.

    Esto es útil si tu teclado tiene mejores sonidos de piano, cuerdas, o percusión que el soundfont por defecto de MuseScore.


    ### Teclado MIDI virtual: cuando no tenés teclado físico

    Si no tenés teclado MIDI, MuseScore incluye un **teclado de piano virtual**:
    1. **Ver → Piano virtual** (o `P` en la barra de herramientas).
    2. Aparece un teclado de piano en pantalla.
    3. Hacé clic en las teclas con el mouse para ingresar notas.

    No reemplaza un teclado físico (es más lento y no detecta velocity), pero es una alternativa viable para practicar el ingreso por paso cuando no tenés hardware.

---

## Actividad en Classroom

### Tarea: S22 — Configuración y uso de teclado MIDI

> **Material necesario**: el docente proporcionará tres archivos: (a) `ejercicio_S22_melodia.mscz`, una partitura de piano en Do mayor, 4/4, 24 compases, completamente VACÍA (solo compases de silencio), lista para recibir una melodía mediante ingreso MIDI; (b) `ejercicio_S22_acordes.mscz`, una partitura de piano en Sol mayor, 3/4, 16 compases con cifrado armónico ya ingresado (G, C, D, Em, Am, Bm) y una línea de bajo escrita, pero SIN los acordes en el pentagrama superior; (c) `ejercicio_S22_partitura.mscz`, una partitura para flauta sola en Fa mayor, 4/4, 32 compases con una melodía rítmicamente variada (corcheas, síncopas, tresillos, puntillos, notas largas) que el estudiante deberá transcribir usando el teclado MIDI.

1. **Conexión y verificación del teclado MIDI.** Conectá tu teclado MIDI a la computadora siguiendo los pasos de la guía (conexión física → encendido → verificación en Preferencias → prueba de funcionamiento). Documentá el modelo de tu teclado, el tipo de conexión usada (USB, MIDI DIN, Bluetooth) y si requirió instalación de drivers. Si no tenés teclado MIDI físico, activá el Piano Virtual de MuseScore (`P`) y documentá que usarás esta alternativa.

2. **Ingreso por paso: melodía desde cero.** Abrí `ejercicio_S22_melodia.mscz`:
    - Activá el modo de ingreso por paso (`N`).
    - Vas a ingresar la siguiente melodía en el pentagrama superior exclusivamente con teclado MIDI (físico o virtual). NO uses el mouse para colocar notas ni las letras A–G:
        - c.1–4: escala ascendente de Do mayor (Do–Re–Mi–Fa–Sol–La–Si–Do) en negras.
        - c.5–8: escala descendente (Do–Si–La–Sol–Fa–Mi–Re–Do) pero en corcheas.
        - c.9–12: arpegio de Do mayor extendido (Do–Mi–Sol–Do₅–Sol–Mi–Do–Mi–Sol) alternando negras y corcheas.
        - c.13–16: una melodía libre de tu invención en Do mayor usando solo negras, corcheas y al menos una blanca.
        - c.17–24: repetí los compases 1–8 pero con la indicación "8va" (tocá todo una octava arriba). Para esto, ingresá las notas normalmente y luego agregá la línea de octava desde la paleta **Líneas → 8va**.
    - Cada nota debe ser ingresada con el teclado MIDI en step-time. Cronometrate: ¿cuánto tiempo te tomó completar los 24 compases?

3. **Ingreso de acordes con teclado MIDI.** Abrí `ejercicio_S22_acordes.mscz`:
    - Observá el cifrado armónico existente (G, C, D, Em, Am, Bm) y el bajo escrito en el pentagrama inferior.
    - En el pentagrama superior, construí los acordes completos sobre cada cambio de armonía usando el teclado MIDI:
        - Tocá simultáneamente las notas de cada acorde (tríada) en el teclado.
        - Asegurate de que las notas del acorde estén dentro del ámbito del pentagrama superior (Do₄–Sol₅) y no choquen con el bajo.
    - Ingresá al menos 5 acordes usando ingreso simultáneo (todas las notas del acorde a la vez) y al menos 5 usando ingreso nota por nota (`Shift` mientras tocás cada nota adicional).
    - Verificá que cada acorde corresponda al cifrado armónico indicado.

4. **Ingreso en tiempo real: transcripción rítmica.** Abrí `ejercicio_S22_partitura.mscz`:
    - La partitura contiene una melodía para flauta rítmicamente variada que DEBÉS transcribir usando ingreso en tiempo real automático.
    - Configurá el metrónomo a un tempo que puedas manejar (sugerencia: empezar en 60 BPM).
    - Activá el modo de ingreso en tiempo real y tocá la melodía con el teclado MIDI siguiendo el metrónomo.
    - Al terminar, revisá el resultado: ¿MuseScore transcribió correctamente los ritmos? ¿Los tresillos se interpretaron bien? ¿Las síncopas?
    - Si el resultado tiene errores, ajustá la cuantización (probar con "semicorchea" en lugar de "corchea") y repetí la grabación.
    - Documentá cuántos intentos necesitaste para obtener una transcripción aceptable.

5. **Integración: método mixto.** Creá una NUEVA partitura desde cero: `APELLIDO_Nombre_S22_mixto.mscz`.
    - Plantilla: Piano. Tonalidad: Re mayor (2 sostenidos). Compás: 4/4. 20 compases.
    - **Compases 1–8 (ingreso por paso con MIDI)**: escribí una melodía en la mano derecha usando exclusivamente ingreso por paso. La melodía debe incluir al menos: 4 corcheas consecutivas, 1 tresillo de corcheas, 2 notas con puntillo, y 1 síncopa (nota ligada a través de la línea divisoria del compás).
    - **Compases 9–16 (ingreso en tiempo real con MIDI)**: continuación de la melodía anterior, pero ingresada en tiempo real automático. La melodía debe ser más fluida y cantabile (apta para tocar de corrido). Grabala con el metrónomo a un tempo cómodo.
    - **Compases 17–20 (acordes con MIDI)**: agregá acordes en la mano izquierda (redondas) usando ingreso simultáneo de acordes con el teclado MIDI. Progresión: I (Re) → V (La) → vi (Sim) → IV (Sol) → I (Re). Ingresá también el cifrado armónico (`Ctrl + K`) sobre cada acorde.
    - Exportá como PDF.

6. **Reflexión sobre ingreso MIDI.** En Classroom, respondé:
    - ¿Qué modo de ingreso (step-time, real-time automático, real-time manual) te resultó más eficiente y por qué? Si no tenés teclado MIDI físico y usaste el piano virtual, ¿cómo afectó eso tu experiencia?
    - ¿Qué ventajas tiene ingresar acordes con teclado MIDI en comparación con hacerlo con el mouse y el teclado de la computadora?
    - Si tuvieras que transcribir una partitura de 100 compases para orquesta completa, ¿usarías ingreso por paso o en tiempo real? Justificá tu elección considerando precisión, velocidad y esfuerzo.

### Entregables

- [ ] `APELLIDO_Nombre_S22_melodia_v01.mscz` (melodía ingresada con teclado MIDI)
- [ ] `APELLIDO_Nombre_S22_melodia_v01.pdf`
- [ ] `APELLIDO_Nombre_S22_acordes_v01.mscz` (acordes con ingreso MIDI)
- [ ] `APELLIDO_Nombre_S22_acordes_v01.pdf`
- [ ] `APELLIDO_Nombre_S22_partitura_v01.mscz` (transcripción en tiempo real)
- [ ] `APELLIDO_Nombre_S22_partitura_v01.pdf`
- [ ] `APELLIDO_Nombre_S22_mixto_v01.mscz` (método mixto)
- [ ] `APELLIDO_Nombre_S22_mixto_v01.pdf`
- [ ] Comentario en Classroom con: (a) respuestas a las 3 preguntas de reflexión, (b) modelo de tu teclado MIDI y tipo de conexión usada (o "Piano Virtual" si no tenés teclado), (c) tiempos: cuánto tardaste en los 24 compases de step-time (Parte 2) y cuántos intentos necesitaste para la transcripción en tiempo real (Parte 4)

### Autoevaluación

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Conexión y verificación MIDI | Teclado detectado, configurado y funcionando; modelo y tipo de conexión documentados | Teclado configurado pero con problemas de latencia o sin documentar | Teclado no configurado ni documentado |
| Ingreso por paso | 24 compases completos; cada nota ingresada con MIDI; uso correcto de duraciones; melodía correcta | 16–23 compases o uso parcial del teclado | <16 compases o ingreso sin teclado MIDI |
| Ingreso de acordes | ≥10 acordes con ingreso MIDI; al menos 5 simultáneos y 5 nota por nota; correspondencia con el cifrado | 7–9 acordes o solo un método de ingreso | ≤6 acordes o sin correspondencia con cifrado |
| Ingreso en tiempo real | Transcripción completada; ritmos mayormente correctos (≥80%); documentación de intentos | Transcripción con >20% de errores rítmicos | Transcripción fallida o sin intentos documentados |
| Método mixto | 20 compases completos; secciones claramente diferenciadas por modo de ingreso; tresillo, síncopa y acordes presentes | 15–19 compases o falta algún elemento requerido | <15 compases o sin diferenciación de modos |
| Reflexión | Responde las 3 preguntas con argumentos técnicos; demuestra entender ventajas/desventajas de cada modo | Responde 2 de 3 correctamente | ≤1 respuesta o superficial |

---

*Basado en: MuseScore Studio 4 Handbook — Note input modes (MIDI keyboard), Preferences | https://handbook.musescore.org*
