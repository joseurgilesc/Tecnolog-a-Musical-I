# Guía Docente — Sesión 25: Reproducción como herramienta de revisión

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, sistema de audio con buena calidad (parlantes de estudio o auriculares de monitoreo para la demostración), archivos `ejercicio_S25_errores.mscz` y `ejercicio_S25_mezcla.mscz` preparados por el docente  
**Referencia:** MuseScore Studio Handbook — Sound and Playback: Play mode, Synthesizer, Soundfonts

---

## Objetivo de la sesión

Que el estudiante internalice la reproducción como HERRAMIENTA DE REVISIÓN (no como entretenimiento), aplique un protocolo sistemático de escucha crítica para detectar errores rítmicos, armónicos y de notación que el ojo pasa por alto, domine el mezclador para aislar instrumentos y ajustar balance, y comprenda el rol de los soundfonts en la calidad de la reproducción explorando alternativas al MS Basic por defecto.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S24 + pregunta: ¿cuántas veces escuchás tu partitura antes de entregarla? |
| **Desarrollo** | 30 min | Demostración: protocolo de revisión auditiva en vivo + mezclador + soundfonts |
| **Práctica** | 65 min | Detección auditiva de errores → corrección → mezcla → comparación de soundfonts → exportación MP3 |
| **Cierre** | 15 min | Contraste visual vs. auditivo, puesta en común, entrega |

---

## 1. Apertura — ¿Escuchás o solo mirás?

### Materiales
- Proyector con MuseScore Studio abierto.
- Sistema de audio funcionando y testeado ANTES de la clase. La mitad de esta sesión depende del sonido. Si los parlantes fallan, la sesión se cae.
- Los archivos `ejercicio_S25_errores.mscz` y `ejercicio_S25_mezcla.mscz` publicados en Classroom **antes de la clase**.

### Dinámica

1. **Revisión de S24** (5 min):
   - "¿Alguien hizo el roundtrip de MusicXML? ¿Qué fue lo que más se perdió?" (Formato de página, fuentes.)
   - "¿Qué formato le mandarías a un amigo que usa Finale? ¿Y a uno que solo quiere escuchar? ¿Y a tu director de orquesta?"
   - Rápidamente: "MIDI para máquinas, MusicXML para músicos, PDF para entregar, MP3 para escuchar. ¿Alguna duda sobre eso?"

2. **Pregunta disparadora** (5 min):
   - Preguntar a la clase: "Levanten la mano los que, cuando terminan de escribir una partitura, la ESCUCHAN completa antes de entregarla."
   - La mayoría levanta la mano.
   - "Ahora levanten la mano los que la escuchan CON AURICULARES, un instrumento a la vez, en loop en los pasajes difíciles, a tempo reducido, y toman notas de cada error que encuentran."
   - Casi nadie.
   - "Esa diferencia es la diferencia entre un estudiante y un editor profesional. El editor profesional SABE que sus ojos le mienten. Confía en sus OÍDOS."
   - Proyectar la frase: **"Tus ojos normalizan errores. Tus oídos los delatan."**
   - "Hoy vamos a aprender a escuchar con intención. No a 'oír' la partitura de fondo mientras hacemos otra cosa. A ESCUCHAR con la misma concentración con la que escribimos."

---

## 2. Desarrollo — El oído como corrector

### Secuencia sugerida

1. **El protocolo de revisión auditiva en vivo** (12 min). Con `ejercicio_S25_errores.mscz`:
   - "Esta partitura de ensamble de vientos parece correcta visualmente. Pero tiene errores ESCONDIDOS. Errores que un corrector visual podría pasar por alto. Vamos a encontrarlos CON LOS OÍDOS."
   - **Paso 1 — Escucha general (2 min)**: reproducir la partitura completa a tempo real. NO decir nada. Al terminar: "¿Algo les llamó la atención? ¿Algo 'chocó'?" Escuchar a los estudiantes. Generalmente detectan 1 o 2 cosas muy obvias.
   - **Paso 2 — Escucha por instrumento (3 min)**: usar Solo en la flauta. "Escuchen SOLO la flauta. ¿La melodía es correcta? ¿Hay algo raro?" Reproducir. Luego el oboe. "¿Y el oboe? ¿Notan algo?" Generalmente en este paso empiezan a aparecer errores que en el tutti se enmascaraban.
   - **Paso 3 — Loop en pasajes sospechosos (3 min)**: "En el compás 23 escuché algo extraño. Vamos a poner SOLO los compases 22-25 en loop a tempo 60%." Activar loop, reducir tempo. Reproducir 3-4 veces. "¿Ahora sí? ¿Esa nota del fagot es un Mi♮ o un Mi♭? ¿Con el loop y tempo reducido se dan cuenta?"
   - **Paso 4 — Escucha por pares (2 min)**: "Ahora silenciemos fagot y clarinete. Solo flauta y oboe. ¿Suena bien la relación entre las dos voces superiores? ¿Hay choques armónicos?" Reproducir.
   - **Paso 5 — Transiciones (2 min)**: "Últimos 2 compases de la sección A + primeros 2 de la B. ¿La modulación es fluida?"
   - **Conclusión**: "En 12 minutos de escucha sistemática encontramos más errores que en 2 horas de revisión visual. Esto NO es magia. Es MÉTODO."

2. **El mezclador como bisturí auditivo** (8 min). Con `ejercicio_S25_mezcla.mscz`:
   - "Esta partitura de cuerdas está bien escrita PERO suena horrible. ¿Por qué?"
   - Reproducir 20 segundos. Los estudiantes van a notar que algo está mal.
   - "El problema no está en las notas. Está en la MEZCLA." Abrir el mezclador (`F10`).
   - Señalar problemas típicos:
     - **Volumen**: "El violonchelo está a 100% y los violines a 20%. El chelo TAPA todo. El balance de cuerdas real es: violines I más fuertes, chelo presente pero no dominante, contrabajo como base."
     - **Panorama**: "Todos los instrumentos están en el centro. En una orquesta real, los violines I están a la IZQUIERDA del director, los violines II centro-izquierda, violas centro, chelos centro-derecha, contrabajos DERECHA atrás. El panorama debe REFLEJAR eso."
     - **Soundfont incorrecto**: "El violín I tiene asignado un sonido de... ¿trompeta? Claro, por eso suena raro."
   - Corregir en vivo: ajustar faders, panoramizar, asignar soundfonts correctos.
   - Reproducir de nuevo. "¿Notan la diferencia? Mismas notas. Misma partitura. Pero ahora suena como un quinteto de cuerdas en lugar de como un accidente de tránsito."
   - **Lección**: "La mezcla NO arregla una mala orquestación. Pero una buena orquestación con mala mezcla suena PEOR que una regular con buena mezcla."

3. **Soundfonts: MS Basic vs. el mundo** (10 min). Con la partitura de errores ya corregida (o con una partitura limpia de demostración):
   - "Todo lo que escuchamos hasta ahora usó MS Basic. Es el sonido por defecto. Pero ¿qué pasa si usamos algo mejor?"
   - Si Muse Sounds está instalado: cambiar el soundfont de la flauta de MS Basic a Muse Sounds. Reproducir un fragmento. "¿Escuchan la diferencia? El legato es real, el vibrato es natural, el ataque de la nota es más definido. MS Basic suena 'a computadora'. Muse Sounds suena 'a grabación'."
   - Si NO está instalado: "Muse Sounds requiere descarga aparte. 2 GB. Vale la pena si van a hacer entregas de audio profesionales. Pero para el trabajo diario, MS Basic es suficiente."
   - "¿Puedo usar otros soundfonts?" Mostrar cómo cargar un .sf2 personalizado en Preferencias. "FluidR3, Timbres of Heaven, Virtual Playing Orchestra... hay un mundo de soundfonts gratuitos."
   - **Advertencia**: "Si usan un soundfont personalizado y comparten el .mscz, la otra persona necesita ESE MISMO soundfont instalado. Si no lo tiene, MuseScore vuelve a MS Basic automáticamente. Para ENTREGAS DE AUDIO, siempre exporten a MP3 o WAV: ahí el sonido queda 'congelado' y no depende del soundfont de quien escucha."

---

## 3. Práctica — El laboratorio auditivo

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S25 — Reproducción como herramienta de revisión

**Material**: el docente proporciona dos archivos:

1. **`ejercicio_S25_errores.mscz`**: Partitura para ensamble de vientos (flauta, oboe, clarinete en Si♭, fagot), 40 compases. La partitura debe PARECER correcta visualmente pero contener errores que sean MÁS FÁCILES de detectar auditivamente que visualmente:
   - 2–3 errores de altura (notas equivocadas enarmónicamente: Fa♯ en lugar de Sol♭ en un contexto donde la armonía pide Sol♭). Estos deben ser SUTILES visualmente pero OBVIOS auditivamente.
   - 2 errores rítmicos (una negra en lugar de una corchea con puntillo en un contexto donde el ritmo correcto es claro al escuchar con metrónomo).
   - 2 errores de articulación (staccato escrito en un pasaje que claramente debería ser legato, o viceversa).
   - 2 errores de omisión de alteración (un Fa que debería ser Fa♯ por la armadura de cortesía de un pasaje modulante).
   - Al menos 1 error que sea MUY DIFÍCIL de ver visualmente (ej. una voz duplicada incorrectamente en un acorde denso).
   - Total: 9–10 errores deliberados.

2. **`ejercicio_S25_mezcla.mscz`**: Partitura para quinteto de cuerdas (violín I, violín II, viola, violonchelo, contrabajo), 32 compases en Re menor, 3/4. Errores de mezcla deliberados:
   - Volúmenes desbalanceados (chelo al máximo, violines al mínimo, contrabajo al 30%).
   - Panorama incorrecto (todos al centro, o instrumentos en posiciones no orquestales).
   - Al menos un instrumento con soundfont incorrecto (viola usando sonido de clarinete, o similar).

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Aplicar el protocolo de revisión auditiva (5 pasos) y documentar errores encontrados en la tabla.
2. Corregir TODOS los errores detectados.
3. Diagnosticar y corregir la mezcla del quinteto de cuerdas.
4. Probar al menos 2 soundfonts diferentes, exportar MP3s comparativos, escribir reflexión.
5. Preguntas de reflexión sobre revisión auditiva.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Detección auditiva | ≥8 errores detectados, tabla documentada, corrección completa | 5–7 errores | ≤4 errores |
| Protocolo de revisión | 5 pasos aplicados sistemáticamente con anotaciones | 3–4 pasos | ≤2 pasos |
| Mezcla y balance | Volumen, pan y soundfonts corregidos; diagnóstico documentado | Correcciones parciales | Sin corrección |
| Soundfonts | 2+ soundfonts comparados; MP3s exportados; reflexión | Un solo soundfont | Sin comparación |
| Reflexión | 3 respuestas con ejemplos concretos, conciencia de limitaciones y justificación | 2 respuestas | ≤1 respuesta |

---

## 4. Cierre — Confiá en tus oídos

### Revisión por parejas (8 min)

- Intercambiar la tabla de detección de errores: "¿Tu compañero encontró errores que vos no? ¿Detectó los mismos con el oído o los vio visualmente? ¿Hay algún error que AMBOS pasaron por alto?"
- Intercambiar los MP3s con diferentes soundfonts: "¿Notás la diferencia entre MS Basic y Muse Sounds? ¿Cuál preferís? ¿Vale la pena el espacio extra en disco?"

### Puesta en común (7 min)

- "Levanten la mano los que encontraron al menos 1 error que JAMÁS habrían visto solo leyendo la partitura." (Estadística. Casi todos.)
- "¿Cuál fue el paso más efectivo del protocolo de revisión? ¿La escucha por instrumento en solo? ¿El loop a tempo reducido? ¿Las transiciones?"
- "¿Alguien encontró que la revisión auditiva le tomó DEMASIADO tiempo? ¿Sienten que es un lujo que no siempre se pueden dar?" Discusión: la revisión auditiva es inversión de tiempo, no gasto. 10 minutos de escucha sistemática ahorran horas de correcciones posteriores (y vergüenza en clase).

### Resumen del docente (5 min)

1. **La reproducción NO es un premio por haber terminado.** Es una herramienta de trabajo. Escuchar tu partitura debería ser lo PRIMERO que hacés al terminar un borrador, no lo último "si sobra tiempo".
2. **El protocolo de revisión auditiva no es opcional para el trabajo profesional.** En cinco pasos (general → por instrumento → por pares → loop focalizado → transiciones) cubrís el 90% de los errores que otras personas encontrarían en tu partitura. Es un método. No es "escuchar a ver qué onda".
3. **El mezclador es tu aliado, no un juguete.** Silenciar, poner en solo, ajustar volumen relativo, panoramizar: son acciones de ANÁLISIS, no de producción musical. Estás usando el mezclador como los médicos usan el estetoscopio: para aislar y diagnosticar.
4. **El soundfont importa.** MS Basic es funcional. Muse Sounds es profesional. Los soundfonts de terceros son un universo por explorar. Pero NUNCA uses "el soundfont no era bueno" como excusa para no revisar. La revisión auditiva funciona incluso con el sonido más básico: una nota equivocada suena mal en MS Basic, en Muse Sounds y en un piano de juguete.
5. **Tus ojos te mienten. Tus oídos no.** El cerebro humano está cableado para encontrar patrones visuales y completar lo que falta. Por eso leemos "Felíz Navidad" aunque diga "Felíz Navdiad". En una partitura, tu cerebro HACE LO MISMO: ve lo que ESPERA ver, no lo que REALMENTE está escrito. La única defensa contra ese sesgo es otro sentido: el oído.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| La reproducción no suena (silencio total) | Verificar que el sintetizador esté funcionando. Ir a **Editar → Preferencias → Audio** y hacer clic en "Probar". Si no suena: (a) en Windows verificar el driver de audio (preferir MME si ASIO no funciona), (b) en Mac verificar que MuseScore tenga permiso de audio en Preferencias del Sistema → Privacidad → Micrófono, (c) verificar que el volumen del sistema no esté en 0 y que los parlantes/auriculares estén conectados. Si el test suena pero la partitura no: verificar que el mezclador no tenga TODOS los canales en mute. |
| Muse Sounds no aparece como opción | Verificar que Muse Hub esté instalado y que los sonidos se hayan descargado COMPLETAMENTE. Si la descarga se interrumpió, puede aparecer como "instalado" pero no funcional. En Muse Hub: **Sonidos → Muse Sounds → Reinstalar**. Después de instalar, REINICIAR MuseScore completamente (cerrar y abrir). Si aún no aparece: en MuseScore, ir a **Editar → Preferencias → Audio → Soundfont** y verificar que la ruta de Muse Sounds esté en la lista. Si no está, agregarla manualmente (ruta típica en Windows: `C:\ProgramData\Muse Hub\downloads`, en Mac: `/Users/[usuario]/Library/Application Support/Muse Hub/downloads`). |
| La exportación a MP3 produce un archivo de 0 bytes o corrupto | Si el sintetizador no puede procesar la partitura (partitura extremadamente larga, muchos instrumentos), la exportación puede fallar. Solución: exportar en partes (mitad de la partitura primero, luego la otra mitad) o reducir el tempo. También verificar espacio en disco. Si el error persiste: exportar como WAV primero (sin compresión) y luego convertir a MP3 con una herramienta externa (Audacity, ffmpeg). |
| Los auriculares de los estudiantes tienen mala calidad y no distinguen los errores sutiles | Permitir que usen los parlantes del aula si son de mejor calidad. Recordar que para detectar errores de altura y armonía la fidelidad NO es crítica: incluso con auriculares baratos, una nota equivocada en un acorde se detecta. La mala calidad afecta más al balance y al timbre que a la corrección de las notas. |
| El estudiante "no escucha nada raro" en la partitura con errores | Esto es una barrera de entrenamiento auditivo, no técnica. Algunos estudiantes aún no han desarrollado el oído para detectar disonancias sutiles. Estrategia: (a) mostrar el error visualmente, (b) reproducir el compás con y sin el error en loop para que comparen, (c) pedirles que canten la línea melódica (si pueden cantarla correctamente pero suena mal en MuseScore, el error está confirmado). Con práctica, el oído se entrena. |
| El mezclador es abrumador para estudiantes sin experiencia en audio | Simplificar: "Ignoren EQ, reverb y efectos. Solo necesitan 3 cosas: el fader de volumen (barra vertical), el botón de Solo (S) y el botón de Mute (M). Para esta sesión, solo necesitan saber silenciar, aislar y ajustar volumen." El resto del mezclador es para sesiones posteriores o para estudiantes con interés en producción. |
| Al cambiar el soundfont, la partitura se reproduce con delay o cortes | El soundfont nuevo puede ser más pesado que MS Basic y exigir más CPU. Solución: (a) aumentar el tamaño del buffer de audio (**Preferencias → Audio → Tamaño del buffer**) a 1024 o 2048 samples, (b) cerrar otras aplicaciones para liberar CPU, (c) si el problema persiste, volver a MS Basic y hacer la comparación de soundfonts en una computadora más potente. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Play mode](https://handbook.musescore.org/sound-and-playback/play-mode.md)
- [MuseScore Studio Handbook — Synthesizer](https://handbook.musescore.org/sound-and-playback/synthesizer.md)
- [MuseScore Studio Handbook — Soundfonts](https://handbook.musescore.org/sound-and-playback/soundfonts.md)
- [MuseScore Studio Handbook — Mixer](https://handbook.musescore.org/sound-and-playback/mixer.md)
- [Muse Hub — descarga oficial](https://www.musehub.com/)
- **Preparación del archivo `ejercicio_S25_errores.mscz`**: crear un ensamble de vientos (flauta, oboe, clarinete en Si♭, fagot) de 40 compases. Componer una pieza corta en tres secciones (A-B-A') con textura contrapuntística ligera. La pieza debe ser MUSICALMENTE coherente (no un caos aleatorio). Luego introducir 9–10 errores: (a) 2–3 errores de altura con alteraciones sutiles (Fa♮ que debería ser Fa♯ por modulación a Sol mayor), (b) 2 errores rítmicos (corchea en lugar de corchea con puntillo en un pasaje de ritmo punteado consistente), (c) 2 errores de articulación (staccato en lugar de legato en una melodía cantabile), (d) 2 omisiones de alteración (nota sin alteración en un compás donde la armonía claramente la requiere), (e) 1 error de duplicación armónica (en un acorde del fagot, duplicar la 3ra del acorde en lugar de la fundamental, creando un hueco textural). La dificultad debe ser MODERADA: los errores deben ser DETECTABLES por un estudiante que aplica el protocolo de escucha sistemática, no imposibles. No usar disonancias extremas: el objetivo es que aprendan a ESCUCHAR, no a sufrir.
- **Preparación del archivo `ejercicio_S25_mezcla.mscz`**: crear un quinteto de cuerdas (violín I, violín II, viola, violonchelo, contrabajo) en Re menor, 3/4, 32 compases. Escribir una pieza correcta musicalmente. Luego, en el mezclador: (a) violín I volumen 20%, violín II 15%, viola 25%, violonchelo 100%, contrabajo 30% (el chelo tapa todo), (b) todos con pan al centro, (c) viola con soundfont de clarinete (o fagot). Guardar el archivo. El sonido debe ser DESAGRADABLE pero las notas deben ser correctas: el problema es de mezcla, no de composición.
- Dato curioso: la práctica de revisar partituras escuchando la reproducción era CIENCIA FICCIÓN hace 30 años. Antes de los editores de partituras con reproducción integrada (años 90), un compositor solo podía "escuchar" su obra imaginándola en su cabeza (audición interna) o pagando músicos para que la tocaran. La reproducción por computadora democratizó la revisión auditiva: hoy cualquier estudiante puede escuchar su sinfonía completa con una orquesta virtual antes de que un solo músico real la haya visto. Beethoven, que era sordo al final de su vida, dependía COMPLETAMENTE de su audición interna. Hoy tenemos una herramienta que él habría matado por tener.
- Dato curioso: el formato SoundFont (.sf2) fue creado por Creative Labs en los años 90 para sus tarjetas de sonido Sound Blaster. Era un formato pensado para videojuegos y multimedia, no para música académica. Tres décadas después, es el estándar de facto para la reproducción de partituras. La industria de la música dio un rodeo: del MIDI hardware de los 80, al SoundFont de los 90, al sampling profesional de los 2000, y de vuelta al SoundFont (ahora con samples de altísima calidad) en los editores de partituras modernos.
- Ejercicio opcional de ampliación (para estudiantes con interés en tecnología musical): descargar el soundfont FluidR3_GM.sf2, cargarlo en MuseScore, y comparar sistemáticamente 5 instrumentos (flauta, oboe, trompeta, violín, piano) entre MS Basic y FluidR3. Crear una tabla comparativa con columnas: Instrumento, Característica (ataque, sustain, vibrato, realismo general), MS Basic (puntaje 1–5), FluidR3 (puntaje 1–5), Comentario. Esto introduce el concepto de "evaluación crítica de librerías de sonido", una habilidad valiosa para quienes se dediquen a la composición con medios digitales.

---

*Guía docente — Tecnología Musical I | Sesión 25*
