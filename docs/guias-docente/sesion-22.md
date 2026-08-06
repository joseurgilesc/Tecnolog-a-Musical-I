# Guía Docente — Sesión 22: Configuración y uso de teclado MIDI

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, teclado MIDI (al menos uno para demostración en clase), archivos `ejercicio_S22_melodia.mscz`, `ejercicio_S22_acordes.mscz` y `ejercicio_S22_partitura.mscz` preparados por el docente  
**Referencia:** MuseScore Studio Handbook — Note input modes (MIDI keyboard), Preferences

---

## Objetivo de la sesión

Que el estudiante conecte y configure correctamente un teclado MIDI con MuseScore Studio, domine el ingreso por paso (step-time) como método principal de trabajo, experimente el ingreso en tiempo real (real-time) comprendiendo la relación entre velocidad de interpretación y precisión rítmica, e integre ambos métodos en un flujo de trabajo mixto que maximice la productividad según la complejidad del material musical.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S21 + pregunta disparadora: ¿el teclado MIDI graba sonido o instrucciones? |
| **Desarrollo** | 30 min | Demostración: conexión MIDI → step-time → acordes → real-time → atajos MIDI |
| **Práctica** | 65 min | Step-time de melodía → acordes con MIDI → transcripción en tiempo real → método mixto |
| **Cierre** | 15 min | Comparación de tiempos, puesta en común, entrega |

---

## 1. Apertura — ¿El MIDI graba sonido?

### Materiales
- Proyector con MuseScore Studio abierto.
- Teclado MIDI conectado y funcionando (verificar ANTES de la clase).
- Los archivos `ejercicio_S22_melodia.mscz`, `ejercicio_S22_acordes.mscz` y `ejercicio_S22_partitura.mscz` publicados en Classroom **antes de la clase**.

### Dinámica

1. **Revisión rápida de S21** (5 min):
   - ¿Recordás cómo transponer un instrumento transpositor? ¿Qué pasa con el sonido y la notación al activar/desactivar "altura de concierto"?
   - ¿Lograron escribir para saxofón y trompeta sin que las notas sonaran mal en la reproducción?
   - Breve mención de que hoy cambiamos de tema completamente: del mundo de los instrumentos transpositores al mundo del hardware y la entrada de datos.

2. **Preguntas disparadoras** (5 min):
   - Proyectar una partitura vacía. Conectar el teclado MIDI en vivo. Tocar una nota. "¿Qué acaba de pasar? ¿El teclado grabó sonido? ¿O envió algo diferente?"
   - Debatir la diferencia entre MIDI y audio: el 90% de los estudiantes confunde ambos conceptos al inicio. "MIDI no es audio. Es una partitura digital."
   - "Levanten la mano quienes tienen teclado MIDI en casa... ¿Cuántos lo usan regularmente con MuseScore? ¿Cuántos lo dejaron guardado en un armario porque 'no supieron configurarlo'?" (Esto genera identificación: muchos compraron un teclado MIDI "porque todo el mundo lo tiene" y nunca lo configuraron correctamente.)

---

## 2. Desarrollo — Del cable al pentagrama

### Secuencia sugerida

1. **¿Qué es MIDI? Desmitificando el protocolo** (6 min). Sin abrir MuseScore aún:
   - Dibujar en el pizarrón dos esquemas: uno de AUDIO (micrófono → grabación → archivo WAV) y otro de MIDI (tecla → instrucción "Do₄, velocity 100" → software → sonido).
   - "MIDI es como un director de orquesta que da instrucciones a los músicos. El director no hace sonido. Los músicos SÍ."
   - Mostrar la diferencia de tamaño: un archivo MIDI de la Quinta Sinfonía de Beethoven cabe en un diskette de 1990. El MP3 de la misma sinfonía no cabe en 50 disketes.
   - **Pregunta clave**: "Si MIDI no es audio, ¿por qué cuando toco el teclado MIDI ESCUCHO algo?" (Porque MuseScore u otro software RECIBE el MIDI y GENERA el audio. El sonido NO viene del teclado, viene de la computadora.)
   - "El teclado MIDI es un controlador. Como el mouse de la computadora: el mouse no 'dibuja' el cursor, le dice a la computadora hacia dónde moverlo."

2. **Conexión del teclado: la ceremonia de los 3 pasos** (7 min). En vivo, con el proyector:
   - **Paso 1 — Físico**: mostrar el cable USB, el puerto en el teclado, el puerto en la computadora. Conectar en vivo.
   - **Paso 2 — Software**: abrir Preferencias → Audio y MIDI → Entrada MIDI. Mostrar la lista de dispositivos. Señalar cuál es el teclado. "Si no aparece, estas son las 4 causas más comunes." (Enumerarlas: teclado apagado, cable dañado, drivers faltantes, MuseScore abierto antes de conectar.)
   - **Paso 3 — Prueba**: activar ingreso (`N`), tocar una nota. "Si aparece la nota en el pentagrama, funciona. Si no, volvemos al Paso 2."
   - **Diagnóstico en vivo**: deliberadamente "olvidar" encender el teclado antes de buscar en Preferencias. "¿Ven? No aparece. Así es como el 80% de los frustrados abandonan. No es que 'no funciona'. Es que falta un paso."

3. **Ingreso por paso: precisión quirúrgica** (9 min). Sobre el archivo `ejercicio_S22_melodia.mscz`:
   - Escribir 4 compases de melodía en vivo usando step-time: seleccionar negra (`5`), tocar Do en el teclado MIDI, seleccionar corchea (`4`), tocar Re, etc.
   - "Observen que NO importa a qué velocidad toco la tecla. MuseScore no está escuchando el ritmo. Solo está escuchando QUÉ tecla presioné. El ritmo lo decido YO con los atajos de duración."
   - Introducir los atajos de productividad: `R` (repetir), `Q` (mitad de duración), `W` (doble de duración), `.` (puntillo), `T` (ligadura).
   - **Demostración de velocidad**: escribir una escala de 2 octavas en step-time. Cronometrar. "En 30 segundos, 16 notas perfectamente colocadas. Con el mouse, esto tomaría 2 minutos."
   - Mostrar el ingreso de acordes: tocar 3 teclas simultáneamente (Do, Mi, Sol) → las tres notas aparecen apiladas. "Ingresar una tríada lleva el mismo tiempo que ingresar una nota suelta. Con el mouse, necesitarías 3 clics."
   - **Pregunta**: "¿Qué pasa si suelto una tecla antes que las otras?" (MuseScore toma las notas que están presionadas en el momento de la inserción. Si soltás Mi antes, solo entran Do y Sol.)

4. **Ingreso en tiempo real: velocidad vs. precisión** (8 min). Sobre el archivo `ejercicio_S22_partitura.mscz`:
   - "Ahora vamos a hacer lo contrario: yo TOCARÉ la melodía al ritmo del metrónomo y MuseScore la transcribirá automáticamente."
   - Configurar tempo a 80 BPM. Activar ingreso en tiempo real. Tocar una melodía simple (negras y corcheas) junto al metrónomo.
   - Mostrar el resultado: "¿Ven? Las blancas están perfectas, las negras también. Pero esa corchea del final... MuseScore la escribió como una negra. ¿Por qué?" (Porque la toqué un poco larga y la cuantización redondeó a la figura más cercana.)
   - Tocar la misma melodía pero MÁS RÁPIDO (tempo 120). Mostrar el resultado: ritmos imprecisos, notas fusionadas, silencios inesperados. "A mayor velocidad, mayor probabilidad de errores de transcripción."
   - Tocar la misma melodía con cuantización más fina (semicorchea en lugar de corchea). "Ahora es más precisa pero más sensible a pequeñas imprecisiones."
   - **Conclusión**: "El ingreso en tiempo real es un atajo, no una solución mágica. Si tocás con precisión, funciona. Si no, el step-time es tu amigo."
   - Mostrar el híbrido: timepo real manual. "Yo decido la duración (`5` para negra) y toco la tecla al ritmo del metrónomo. MuseScore inserta MI duración en MI momento rítmico."

---

## 3. Práctica — El teclado MIDI como herramienta

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S22 — Configuración y uso de teclado MIDI

**Material**: el docente proporciona tres archivos:

1. **`ejercicio_S22_melodia.mscz`**: Partitura para piano en Do mayor, 4/4, 24 compases, completamente VACÍA. Solo compases de silencio. El pentagrama superior listo para recibir la melodía de la Parte 2 de la actividad. El pentagrama inferior vacío (no se usa en esta parte). Entregar sin contenido: solo estructura de compases.

2. **`ejercicio_S22_acordes.mscz`**: Partitura para piano en Sol mayor (1 sostenido), 3/4, 16 compases. Pentagrama superior vacío. Pentagrama inferior con una línea de bajo en redondas: G₂, C₃, D₃, G₂, Em₂, Am₂, Bm₂, C₃, G₂, D₃, Em₂, Am₂, Bm₂, C₃, D₃, G₂. Cifrado armónico (`Ctrl + K`) ya ingresado sobre el primer tiempo de cada compás: G, C, D, G, Em, Am, Bm, C, G, D, Em, Am, Bm, C, D, G. SIN acordes construidos en el pentagrama superior.

3. **`ejercicio_S22_partitura.mscz`**: Partitura para flauta sola en Fa mayor (1 bemol), 4/4, 32 compases. Melodía con variedad rítmica deliberada: incluye corcheas, síncopas (ligaduras a contratiempo), tresillos de corchea, notas con puntillo, blancas, y silencios de negra. Ámbito: Fa₄–Fa₆. La partitura está COMPLETA. El estudiante NO la modifica, solo la usa como referencia para transcribir. La transcripción se hace en una copia nueva (el estudiante crea una partitura desde cero o duplica el archivo y borra las notas).

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Conectar, verificar y documentar teclado MIDI.
2. Ingresar melodía de 24 compases por step-time.
3. Ingresar acordes con MIDI (simultáneo y nota por nota).
4. Transcribir melodía rítmicamente compleja en tiempo real.
5. Crear partitura con método mixto integrando los 3 modos de ingreso.
6. Reflexionar sobre eficiencia y casos de uso.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Conexión y configuración | Teclado detectado y funcionando; modelo y conexión documentados; prueba exitosa | Configurado pero sin documentar o con latencia | Teclado no configurado |
| Ingreso por paso | 24 compases completados con step-time MIDI; uso correcto de atajos de duración; melodía correcta | Parcialmente completado o uso limitado de MIDI | Sin uso de teclado MIDI |
| Ingreso de acordes | ≥10 acordes con MIDI (simultáneo y nota por nota); correspondencia con cifrado | 7–9 acordes o un solo método | ≤6 acordes |
| Transcripción en tiempo real | Transcripción con ≥80% de precisión rítmica; intentos documentados; ajuste de cuantización probado | <80% de precisión o sin ajuste de parámetros | Transcripción fallida |
| Método mixto | Las 3 secciones completas y diferenciadas; elementos rítmicos requeridos presentes | 2 secciones completas o falta algún elemento | 1 sección o método mixto no evidenciable |
| Reflexión | 3 respuestas con argumentos técnicos y comparación de modos | 2 respuestas correctas | ≤1 respuesta |

---

## 4. Cierre — MIDI es el idioma, no el sonido

### Revisión por parejas (8 min)

- Intercambiar la transcripción en tiempo real (Parte 4): "Reproducí la transcripción del compañero. ¿Suena igual que el original? ¿Dónde están las diferencias rítmicas?"
- "Compará los tiempos de step-time (Parte 2). ¿Quién fue más rápido? ¿Qué atajos usó?" (Fomenta competencia amistosa y aprendizaje de atajos entre pares.)

### Puesta en común (7 min)

- "¿Cuántos lograron una transcripción en tiempo real 'perfecta' al primer intento? ¿Al segundo? ¿Al quinto?" (Estadística rápida. Generalmente muy pocos al primer intento. Esto valida la dificultad real del ingreso en tiempo real.)
- "Si tuvieran que escribir una partitura de 200 compases, ¿usarían step-time o real-time? ¿Por qué?" (Discusión: step-time es más lento pero más seguro para material complejo. Real-time es excelente para borradores rápidos o melodías simples. La respuesta madura: depende del material.)
- "¿Qué fue más difícil de aceptar: que el teclado MIDI no produce sonido, o que el ingreso en tiempo real no es 'mágico'?" (Discusión conceptual.)

### Resumen del docente (5 min)

1. **MIDI NO es audio.** MIDI es instrucciones: qué nota, con qué fuerza, cuánto dura. Quien entiende esta diferencia entiende el 80% de la tecnología musical. No es un detalle técnico: es un CONCEPTO FUNDACIONAL.
2. **El ingreso por paso es el método de producción profesional.** Es más lento pero produce resultados perfectos. El 90% de los transcriptores profesionales y copistas usan step-time para trabajo serio. El real-time es para bocetos e ideas rápidas.
3. **El teclado MIDI acelera TODO.** Incluso en step-time, ingresar notas con un teclado MIDI es 3–5 veces más rápido que con el mouse. Si van a usar MuseScore seriamente, un teclado MIDI (aunque sea de 25 teclas y económico) es la mejor inversión.
4. **La cuantización es un cuchillo de doble filo.** Demasiada cuantización = música robótica. Muy poca = caos rítmico. El punto justo depende del estilo musical. Una balada admite menos cuantización que un pasaje de semicorcheas en un allegro.
5. **Conectar el teclado son 3 pasos, no 30.** Físico, software, prueba. Si falla, es uno de esos 3. El problema NUNCA es "MuseScore no funciona con mi teclado". Siempre es un paso omitido.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| El teclado no aparece en la lista de dispositivos MIDI | Diagnóstico sistemático: (1) ¿está encendido? Ver switch. (2) ¿cable USB funciona? Probar otro. (3) ¿MuseScore se abrió antes de conectar? Cerrar y reabrir. (4) ¿necesita drivers? Verificar en web del fabricante. (5) ¿el puerto USB entrega energía? Probar otro puerto o un hub alimentado. En Mac, verificar en `/Aplicaciones/Utilidades/Configuración de Audio MIDI.app` que el dispositivo aparezca. |
| El estudiante no tiene teclado MIDI físico | Activar Piano Virtual (`P`). Explicar que pierde velocidad y expresión pero gana comprensión del flujo de trabajo. Para la evaluación, el Piano Virtual es aceptable pero debe documentarse como tal. |
| Latencia alta: el sonido "llega tarde" al tocar | En Mac (CoreAudio): generalmente no hay problema. En Windows: instalar ASIO4ALL (driver gratuito de baja latencia) o seleccionar el driver WASAPI en Preferencias de Audio. Reducir el buffer a 128–256 samples. Si persiste, usar el sintetizador interno del teclado MIDI como salida. |
| El ingreso en tiempo real produce un desastre rítmico | Reducir el tempo (40–60 BPM). Aumentar la cuantización a "negra" para que MuseScore ignore las subdivisiones finas. Si aún falla, cambiar a real-time manual donde el estudiante elige la duración. Si todo falla: step-time. No hay vergüenza en usar step-time; lo usan los profesionales. |
| El estudiante ingresa acordes y solo aparece UNA nota | Está soltando las teclas antes de que MuseScore registre el acorde. Solución: mantener presionadas TODAS las teclas del acorde simultáneamente hasta que las notas aparezcan en el pentagrama. Para ingreso nota por nota: mantener `Shift` mientras se agregan notas adicionales. |
| El teclado "inventa" notas (notas dobles, repeticiones) | Generalmente es un problema de "bouncing" del teclado (contactos sucios o desgastados). Probar con otro software MIDI para confirmar. Si es el teclado, requiere reparación física. Temporalmente, limpiar el contacto o ajustar la sensibilidad en la configuración del teclado. |
| Confusión entre velocity y dinámica | La velocity (0–127) es el dato MIDI crudo. La dinámica (pp, mf, ff) es la interpretación musical. En MuseScore, la velocity se traduce automáticamente en dinámica, pero no son lo mismo. Podés tener una nota con velocity 100 y marcarla *piano*; MuseScore respetará tu marca de dinámica. |
| El estudiante quiere usar el teclado MIDI para cambiar instrumentos durante la reproducción | No es el flujo correcto. El teclado MIDI en MuseScore es para ENTRADA de datos, no para PERFORMANCE en vivo. Para cambiar instrumentos durante la reproducción, se usan los Canales MIDI en el Mezclador (`F10`), no el teclado físico. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Note input modes](https://handbook.musescore.org/basics/note-input.md)
- [MuseScore Studio Handbook — Keyboard shortcuts](https://handbook.musescore.org/basics/keyboard-shortcuts.md)
- [MuseScore Studio Handbook — Preferences](https://handbook.musescore.org/basics/preferences.md)
- **Preparación del archivo `ejercicio_S22_melodia.mscz`**: crear partitura para piano en Do mayor, 4/4, 24 compases. Ambos pentagramas completamente vacíos (solo silencios de compás). El pentagrama superior en clave de Sol, el inferior en clave de Fa. No incluir ninguna nota. El archivo mínimo posible: partitura nueva desde plantilla Piano, 24 compases, guardar sin ingresar nada.
- **Preparación del archivo `ejercicio_S22_acordes.mscz`**: crear partitura para piano en Sol mayor, 3/4, 16 compases. Ingresar el bajo en el pentagrama inferior: redondas en G₂, C₃, D₃, G₂, Em₂, Am₂, Bm₂, C₃, G₂, D₃, Em₂, Am₂, Bm₂, C₃, D₃, G₂. Ingresar cifrado armónico (`Ctrl + K`) sobre el primer tiempo de cada compás: G, C, D, G, Em, Am, Bm, C, G, D, Em, Am, Bm, C, D, G. NO escribir los acordes en el pentagrama superior. El pentagrama superior debe estar completamente vacío.
- **Preparación del archivo `ejercicio_S22_partitura.mscz`**: crear partitura para Flauta sola en Fa mayor, 4/4, 32 compases. Componer una melodía con variedad rítmica explícita: debe incluir al menos 3 tresillos de corchea, 5 síncopas (ligaduras a contratiempo), 8 notas con puntillo, 4 silencios de negra, y combinaciones de corcheas con semicorcheas. Ámbito: Fa₄–Fa₆. La melodía debe ser "tocable" (no un ejercicio aleatorio). Entregar completa: los estudiantes deben transcribirla escuchando y leyendo.
- Dato curioso: el estándar MIDI fue propuesto por primera vez por Dave Smith (fundador de Sequential Circuits) en 1981. En la feria NAMM de 1983, conectaron un sintetizador Sequential Prophet-600 con un Roland Jupiter-6 mediante MIDI. Fue la primera demostración pública de dos instrumentos de diferentes fabricantes comunicándose. La audiencia aplaudió de pie. Ese cable de 5 pines cambió la industria musical para siempre.
- Dato curioso: la velocity MIDI usa valores de 0 a 127 porque el protocolo MIDI original usaba paquetes de 7 bits (2⁷ = 128 valores posibles). Es una limitación histórica, no musical. El nuevo estándar MIDI 2.0 (adoptado en 2020) usa valores de 16 bits (65,536 niveles) y agrega resolución mucho más fina para velocity, pitch bend y controladores. MuseScore aún no soporta MIDI 2.0 (2025).
- Dato curioso: antes del ingreso por computadora, los copistas musicales profesionales escribían partituras A MANO con pluma de tinta china. Un copista experimentado podía escribir 4–6 páginas por día. Hoy, con MuseScore y un teclado MIDI, un transcriptor profesional puede producir 20–30 páginas por día. El MIDI no solo facilitó la música electrónica: revolucionó la COPISTERÍA y la edición de partituras.
- Ejercicio opcional de ampliación (para estudiantes con teclado MIDI y habilidad pianística): entregar una partitura de una invención a dos voces de Bach y pedirles que la transcriban en tiempo real tocando AMBAS voces simultáneamente con las dos manos. Deben asignar la mano derecha a la voz 1 (plica arriba) y la mano izquierda a la voz 2 (plica abajo) en un mismo pentagrama. Es un ejercicio avanzado de coordinación, transcripción y manejo de voces en MuseScore.

---

*Guía docente — Tecnología Musical I | Sesión 22*
