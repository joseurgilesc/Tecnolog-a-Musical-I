# Guía Docente — Sesión 24: Importación y exportación MusicXML

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivos `ejercicio_S24_finale.musicxml`, `ejercicio_S24_desordenado.mscz` y `ejercicio_S24_partitura.mscz` preparados por el docente  
**Referencia:** MuseScore Studio Handbook — File formats (MusicXML), Save/Export/Print

---

## Objetivo de la sesión

Que el estudiante comprenda la diferencia fundamental entre formatos de intercambio (MusicXML, MIDI) y formatos de entrega (PDF, MP3), importe partituras desde otros editores vía MusicXML diagnosticando y corrigiendo las pérdidas típicas de formato, ejecute un flujo completo de exportación multiformato (.mscz, .musicxml, .mxl, .mid, .pdf, .mp3) entendiendo el propósito específico de cada uno, y genere particellas profesionales formateadas para entrega a músicos.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S23 + pregunta disparadora: ¿cómo comparto mi partitura con alguien que usa Finale? |
| **Desarrollo** | 30 min | Demostración: importación MusicXML → exportación multiformato → roundtrip → particellas |
| **Práctica** | 65 min | Importar de Finale → exportar en 6 formatos → roundtrip → particellas → flujo inter-editor |
| **Cierre** | 15 min | Tabla de formatos, puesta en común, entrega |

---

## 1. Apertura — La torre de Babel de las partituras

### Materiales
- Proyector con MuseScore Studio abierto.
- Los archivos `ejercicio_S24_finale.musicxml`, `ejercicio_S24_desordenado.mscz` y `ejercicio_S24_partitura.mscz` publicados en Classroom **antes de la clase**.
- Opcional: tener instalado Finale Notepad (gratuito) o acceso a un editor online (Flat.io, Noteflight) para mostrar el flujo inter-editor en vivo.

### Dinámica

1. **Revisión de S23** (5 min):
   - ¿Alguien logró importar un MIDI propio y limpiarlo? ¿Cuánto tiempo les llevó?
   - ¿Cuál es la diferencia entre Type 0 y Type 1? ¿Cuál es mejor para importar?
   - Rápidamente: ¿MIDI transmite nombre de notas o números de nota? (Números.) Bien. Hoy vemos un formato que SÍ transmite nombres de nota.

2. **Preguntas disparadoras** (5 min):
   - "Imaginen esta situación real: ustedes escribieron una partitura hermosa en MuseScore. Su profesor de composición usa Finale. Les pide que le manden la partitura para corregirla. ¿Qué le mandan?"
   - Opciones que suelen aparecer: PDF (no se puede editar), MIDI (se pierde todo el formato), .mscz (Finale no lo abre). "Ninguna de esas sirve."
   - "Existe un formato que es como el esperanto de las partituras: MusicXML. Todos los editores de partituras lo entienden. MuseScore lo entiende. Finale lo entiende. Sibelius lo entiende. Dorico lo entiende. Flat.io lo entiende."
   - Proyectar la frase: **MIDI es para máquinas. MusicXML es para músicos.**
   - "¿Alguna vez necesitaron mandar una partitura a alguien que usa otro programa? ¿Qué hicieron?" (Escuchar experiencias. Generalmente frustración.)

---

## 2. Desarrollo — El puente entre editores

### Secuencia sugerida

1. **MusicXML vs. MIDI: el contraste definitivo** (6 min). Sin abrir archivos aún:
   - Dibujar en el pizarrón dos columnas: MIDI | MusicXML.
   - "MIDI dice: 'en el tiempo 1.5, nota número 60 con velocity 100, canal 1'. MusicXML dice: 'compás 1, tiempo 2, negra, Do₄, con staccato y dinámica *mf*'."
   - Mostrar el mismo compás en ambos formatos (proyectar un fragmento de XML): "¿Ven la diferencia? MIDI es un cronómetro. MusicXML es una partitura."
   - **Analogía**: "MIDI es las instrucciones de montaje de un mueble IKEA (atornillar A-7 en B-3, girar 90°). MusicXML es la FOTO del mueble armado. Con las instrucciones podés reconstruir el mueble pero no sabés cómo se ve. Con la foto sabés cómo se ve pero no podés reconstruirlo exactamente."
   - "¿Cuál es mejor? Depende. ¿Querés que un robot toque tu música? MIDI. ¿Querés que un humano lea tu partitura en otro programa? MusicXML."

2. **Importación desde Finale/Sibelius** (9 min). Con `ejercicio_S24_finale.musicxml`:
   - "Este archivo fue creado en Finale y exportado como MusicXML. Vean qué pasa cuando lo abro en MuseScore."
   - Abrir el archivo. La partitura aparece instantáneamente.
   - "Vean: las notas están. Las claves están. La armadura está. Las dinámicas están. Las ligaduras están. ¡Esto es INCREÍBLE comparado con importar MIDI!"
   - "Pero... ¿está perfecto?" Hacer zoom. Señalar problemas típicos:
     - **Formato de página**: "Finale usa márgenes diferentes. Los saltos de sistema no coinciden. Los compases quedan apiñados o muy espaciados."
     - **Fuentes**: "Finale usaba Times New Roman para el título. MuseScore usa su propia fuente. El texto se preserva pero se VE diferente."
     - **Posición de dinámicas**: "En Finale, el *mf* estaba más cerca del pentagrama. En MuseScore quedó más lejos."
   - "Esto NO es un error de MuseScore. Es una consecuencia del formato MusicXML: prioriza el CONTENIDO (qué dice) sobre la PRESENTACIÓN (cómo se ve)."
   - Corregir en vivo: reacomodar saltos de página, ajustar márgenes, reposicionar marcas.
   - **Lección clave**: "Importar desde MusicXML es un 90% más rápido que escribir desde cero, pero NUNCA es 100% automático. El 10% de ajuste de formato es inevitable."

3. **Exportación multiformato: un archivo, 7 formatos** (7 min). Con `ejercicio_S24_desordenado.mscz`:
   - "Esta partitura tiene errores de formato a propósito. Antes de compartir algo, SIEMPRE verificamos."
   - Señalar los errores: salto de página que corta una frase, metadatos incompletos, dinámica encimada.
   - "La parte técnica de exportación es trivial: Archivo → Exportar → elegir formato. Lo DIFÍCIL es saber QUÉ formato usar PARA QUÉ."
   - Explicar cada formato con el contexto de uso:

     | Formato | ¿Para quién? | ¿Para qué? |
     |---|---|---|
     | **.mscz** | Para VOS | Tu archivo de trabajo. NUNCA lo mandes por correo si la otra persona no usa MuseScore. |
     | **.musicxml / .mxl** | Para otro MÚSICO con otro editor | "Tomá, abrilo en tu programa y editalo." |
     | **.mid** | Para un PRODUCTOR o DAW | "Tomá, cargalo en tu secuenciador y ponele buenos sonidos." |
     | **.pdf** | Para el DIRECTOR o los MÚSICOS | "Esta es la partitura final para leer en el atril." |
     | **.mp3** | Para CUALQUIERA | "Escuchá cómo suena sin necesidad de instalar nada." |

   - **Demostración del roundtrip** (3 min adicionales):
     - Exportar la partitura corregida como .musicxml.
     - Reabrir ese .musicxml en MuseScore.
     - "Vean: la música está igual. Pero las fuentes cambiaron. Y los saltos de página también."
     - "Esto se llama roundtrip: exportar y reimportar. Idealmente debería ser perfecto. En la práctica, algo se pierde. Saber QUÉ se pierde es parte del oficio."

4. **Particellas: de la partitura completa a las partes individuales** (8 min). Con `ejercicio_S24_partitura.mscz`:
   - "Una partitura de orquesta o ensamble tiene dos versiones: la PARTITURA COMPLETA (el director ve todos los instrumentos) y las PARTICELLAS (cada músico ve SOLO su parte)."
   - Proyectar la partitura completa: "Esto lo lee el director. Tiene 18 pentagramas en cada página."
   - "Pero el flautista NO necesita ver lo que hace el violonchelo. Solo necesita su línea. Eso es una particella."
   - Mostrar cómo generar partes: **Archivo → Partes → Generar todas las partes**.
   - Abrir una parte (ej. Violín I). "Vean: solo la línea de Violín I. Sin distracciones. Con silencios de espera donde no toca."
   - **Formatear la parte** (esto es lo que toma tiempo):
     - Ajustar saltos de página: "El violinista NO quiere pasar la página en medio de una escala rápida. Los saltos de página deben ser en SILENCIOS."
     - Números de compás: "Deben coincidir con la partitura completa. El director dice 'compás 47' y todos encuentran el compás 47 en su parte."
     - Silencios multicompás: "Si el instrumento no toca durante 20 compases, NO escribimos 20 compases de silencio. Escribimos UN bloque que dice '20' y listo."
   - "Generar particellas es fácil. FORMATEAR particellas es un arte. Una particella mal formateada hace que el músico se pierda en el ensayo. Y un músico perdido te va a mirar con odio."

---

## 3. Práctica — El laboratorio de formatos

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S24 — Importación y exportación MusicXML

**Material**: el docente proporciona tres archivos:

1. **`ejercicio_S24_finale.musicxml`**: Partitura de cuarteto de cuerdas (Violín I, Violín II, Viola, Violonchelo) de 24 compases en Re mayor (2 sostenidos), 4/4, exportada desde Finale (o Finale Notepad, o Sibelius First, o cualquier editor que no sea MuseScore). La partitura debe ser musicalmente correcta (notas, ritmos, dinámicas, articulaciones) pero con formato propio del editor original (márgenes, fuentes, espaciado, saltos de sistema propios de Finale/Sibelius). Incluir título y compositor. NO debe ser un archivo generado desde MuseScore y renombrado.

2. **`ejercicio_S24_desordenado.mscz`**: Partitura de MuseScore para piano en Fa mayor (1 bemol), 3/4, 20 compases. Debe tener errores deliberados: (a) 2–3 saltos de página mal puestos (cortan frases musicales), (b) metadatos incompletos (sin compositor, sin título), (c) al menos 2 dinámicas superpuestas con otros elementos, (d) una ligadura rota en un salto de sistema, (e) una alteración enarmónica incorrecta (Sol♯ que debería ser La♭ en el contexto de la pieza). La partitura debe ser MUSICALMENTE correcta (si se reproduce suena bien) pero EDITORIALMENTE descuidada.

3. **`ejercicio_S24_partitura.mscz`**: Partitura para Piano solo en Mi menor (1 sostenido), 4/4, 32 compases. Contenido: una pieza original con mano derecha melódica (negra y corchea, ámbito Si₃–Mi₅) y mano izquierda con acompañamiento de acordes quebrados (corcheas, ámbito Mi₂–Si₃). La pieza debe ser lo suficientemente independiente melódicamente como para que la mano derecha funcione como una línea de flauta separada.

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Importar MusicXML desde Finale y corregir formato.
2. Corregir partitura desordenada y exportar en 6 formatos incluyendo prueba de roundtrip.
3. Generar particellas (flauta + piano) desde la partitura de piano solo.
4. Flujo inter-editor con tabla comparativa de preservación.
5. Reflexión sobre el propósito de cada formato.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Importación MusicXML | ≥5 diferencias identificadas y corregidas; formato profesional | 3–4 diferencias corregidas | ≤2 o sin corrección |
| Exportación multiformato | 6 formatos exportados correctamente; partitura corregida; roundtrip documentado | 4–5 formatos o sin documentar roundtrip | ≤3 formatos |
| Particellas | Partes generadas, formateadas y exportadas como PDF; números de compás y silencios correctos | Partes generadas con errores de formato | Sin particellas |
| Flujo inter-editor | Editor externo usado; MusicXML importado; tabla comparativa completa; diferencias documentadas | Proceso completo pero tabla incompleta | Sin flujo inter-editor |
| Reflexión | 3 respuestas con comprensión de formatos, pérdida y propósito | 2 respuestas correctas | ≤1 respuesta |

---

## 4. Cierre — Cada formato tiene su propósito

### Revisión por parejas (8 min)

- Intercambiar el PDF de las particellas: "¿Podrías leer esta parte en un atril? ¿Los saltos de página son lógicos? ¿Los silencios multicompás son claros?"
- Intercambiar la tabla comparativa del flujo inter-editor: "¿Ambos usaron el mismo editor externo? ¿Encontraron las mismas pérdidas?"

### Puesta en común (7 min)

- "Levanten la mano los que encontraron que el roundtrip (exportar y reimportar MusicXML) perdió ALGO. ¿Qué fue lo que más se perdió?" (Estadística. Generalmente formato de página y fuentes.)
- "Si tuvieran que mandarle una partitura a alguien que NO saben qué programa usa, ¿qué formato le mandan: PDF, MusicXML, MIDI, MP3?" (Discusión: la respuesta madura es MusicXML PORQUE es editable, pero si solo necesita leer → PDF, si solo necesita escuchar → MP3. Depende del contexto.)
- "¿Qué fue más sorprendente: lo bien que funciona MusicXML o lo MAL que funciona en algunas cosas?" (Discusión abierta.)

### Resumen del docente (5 min)

1. **MusicXML es el puente entre islas.** Cada editor de partituras es una isla. MusicXML es el único barco que navega entre todas. Sin MusicXML, tus partituras son prisioneras del programa que las creó.
2. **MIDI y MusicXML NO compiten. Se complementan.** MIDI es para la interpretación (cómo suena). MusicXML es para la notación (cómo se lee). Si los confundís, perdés información. Si los usás correctamente, tu flujo de trabajo es imbatible.
3. **Exportar es fácil. Formatear es el trabajo real.** En 5 segundos exportás a PDF. Pero el PDF solo vale la pena si la partitura está bien formateada. El 80% del trabajo de un editor de partituras NO es escribir notas: es AJUSTAR el formato para que sea legible, profesional y publicable.
4. **Las particellas NO son la partitura completa recortada.** Tienen sus propias reglas: silencios multicompás, saltos de página en silencios, números de compás sincronizados, nombre del instrumento visible. Una particella mal hecha arruina un ensayo. Una particella bien hecha pasa desapercibida (y eso es exactamente lo que querés).
5. **Cada formato tiene un propósito. Usá el correcto para cada situación.** .mscz para trabajar. .mxl para compartir con otros editores. .mid para DAWs. .pdf para entregar. .mp3 para escuchar. No hay UN formato perfecto. Hay EL formato correcto para CADA necesidad.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| El MusicXML de Finale se ve HORRIBLE en MuseScore (formatos completamente rotos) | Revisar la versión de MusicXML exportada desde Finale. Finale antiguo (versiones previas a 2014) exporta MusicXML 2.0 que MuseScore 4 interpreta con limitaciones. Solución: actualizar Finale a una versión reciente, o usar un conversor intermedio. Si no es posible, aceptar que el formateo será manual. |
| El estudiante no tiene acceso a otro editor de partituras (Parte 4 del ejercicio) | Alternativas gratuitas online: Flat.io (plan gratuito permite crear y exportar MusicXML), Noteflight (plan básico gratuito), MuseScore.com (el editor online). También Finale Notepad es gratuito para descarga. Si ninguna opción es viable, el docente puede proporcionar un MusicXML generado desde Finale/Sibelius para que el estudiante haga el proceso inverso (en lugar de crear desde cero en el editor externo). |
| La exportación a MP3 no produce audio o suena a silencio | Verificar que el sintetizador de MuseScore esté funcionando (reproducir la partitura dentro del programa). Si suena dentro de MuseScore pero no en el MP3, revisar la configuración de audio en Preferencias. En Windows, verificar que el mezclador de sonido no tenga muteado a MuseScore. En Mac, verificar los permisos del micrófono (MuseScore no necesita micrófono, pero el sistema a veces lo bloquea). |
| Las particellas muestran compases de silencio en lugar de silencios multicompás | MuseScore inserta silencios multicompás automáticamente cuando detecta bloques largos de silencio. Si no lo hace: seleccionar los compases de silencio → clic derecho → **Propiedades del compás → Silencio multicompás → Activado**. También verificar en **Formato → Estilo → Silencios multicompás** que el número mínimo de compases para agrupar esté configurado correctamente (por defecto 2). |
| Las partes generadas no tienen título ni nombre de instrumento | Las partes heredan el título y subtítulo de la partitura completa. Para el nombre del instrumento: este se genera automáticamente a partir del nombre del pentagrama. Si el pentagrama se llama "Pista 1" en lugar de "Violín I", renombrarlo en **Propiedades del pentagrama**. Para agregar el nombre del instrumento en cada página de la parte: **Estilo → Cabecera y pie de página → nombre del instrumento**. |
| Los números de compás de las particellas no coinciden con la partitura completa | Si hay compases excluidos de la parte (ej. la flauta no toca en los compases 5–12), MuseScore los reemplaza con silencios pero mantiene la numeración. Verificar que no haya compases "ocultos" accidentalmente. Si un compás se eliminó por error de la parte: **Editar → Instrumentos → seleccionar la parte → asegurarse de que esté completa**. |
| La exportación como MusicXML genera un archivo enorme (varios MB) para una partitura simple | Probablemente se está exportando como .musicxml sin comprimir en lugar de .mxl. El .musicxml es texto XML plano (legible pero grande). El .mxl es ZIP comprimido (20× más pequeño). Para compartir, usar SIEMPRE .mxl. Para inspección o procesamiento automatizado, usar .musicxml. |
| Al reimportar el MusicXML en MuseScore, los instrumentos cambiaron (Violín se convirtió en Piano) | El MusicXML incluye el nombre del instrumento, pero si el editor original usó un nombre no estándar ("Violin" sin tilde, "Vln I", etc.), MuseScore puede no reconocerlo. Solución: después de importar, verificar y corregir manualmente la asignación de instrumentos en cada pentagrama. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — File formats](https://handbook.musescore.org/basics/file-formats.md)
- [MuseScore Studio Handbook — Parts](https://handbook.musescore.org/advanced-topics/parts.md)
- [MuseScore Studio Handbook — Save/Export/Print](https://handbook.musescore.org/basics/save-export-print.md)
- [MusicXML official website](https://www.musicxml.com/)
- **Preparación del archivo `ejercicio_S24_finale.musicxml`**: si el docente tiene acceso a Finale (o Finale Notepad gratuito), crear un cuarteto de cuerdas de 24 compases en Re mayor. Completar con melodías independientes en cada voz, dinámicas, articulaciones y texto (título, compositor). Exportar como MusicXML 4.0 sin comprimir. Si no hay acceso a Finale, usar Sibelius First (gratuito), Dorico SE (gratuito), Flat.io (online, exporta MusicXML), Noteflight (online), o MuseScore 3 (exporta MusicXML 3.1 que MuseScore 4 abre, y tendrá diferencias sutiles con la versión nativa de MuseScore 4). El objetivo es que el archivo PROVENGA de otro editor, cualquiera que sea.
- **Preparación del archivo `ejercicio_S24_desordenado.mscz`**: crear una partitura para piano en Fa mayor, 3/4, 20 compases. Escribir una pieza corta musicalmente correcta. Luego introducir los errores deliberadamente: insertar saltos de página en lugares incómodos (`Ctrl + Enter`), borrar el campo de compositor y poner un título genérico, mover dinámicas para que se superpongan con las notas (arrastrar con el mouse), romper una ligadura seleccionándola y moviendo su punto de anclaje, y escribir un Sol♯ que en el contexto de Fa mayor (1 bemol) debería ser La♭.
- **Preparación del archivo `ejercicio_S24_partitura.mscz`**: crear partitura para Piano en Mi menor, 4/4, 32 compases. Componer una pieza con melodía en la mano derecha que sea lo suficientemente independiente como para funcionar como línea de flauta. La mano izquierda debe ser un acompañamiento de acordes quebrados. NO incluir otros instrumentos: la partitura es solo para piano. El ejercicio de las particellas requiere que los estudiantes CREEN el pentagrama de flauta y muevan la melodía.
- Dato curioso: MusicXML fue creado por Michael Good, un programador y músico que hizo su tesis doctoral en Stanford sobre representación digital de partituras en los años 90. Fundó la empresa Recordare (del latín "recordar") en 2000. En 2017, MakeMusic (los creadores de Finale) compraron Recordare y MusicXML. Irónicamente, la empresa que creó uno de los formatos propietarios más cerrados (.mus de Finale) terminó siendo dueña del estándar ABIERTO de intercambio.
- Dato curioso: el nombre "MusicXML" es un juego de palabras. XML = eXtensible Markup Language. Pero "MusicXML" también suena como "musical" en inglés. Michael Good eligió el nombre para que fuera fácil de recordar y tuviera una connotación positiva. Funcionó: MusicXML es hoy el formato de intercambio más usado en notación musical digital.
- Dato curioso: la exportación de particellas era una tarea TITÁNICA antes de los editores digitales. En la era pre-computadora (hasta ~1990), un copista profesional escribía la partitura completa y luego copiaba MANUALMENTE cada parte individual. Para una sinfonía de 40 minutos con 30 instrumentos, extraer las partes tomaba SEMANAS de trabajo. Hoy, MuseScore genera las 30 partes en menos de 5 segundos. El formateo sigue llevando horas, pero la extracción es instantánea. Los copistas del siglo XIX nos mirarían con envidia (y un poco de rencor).
- Ejercicio opcional de ampliación (para estudiantes avanzados o con interés editorial): crear una partitura de 4 páginas en MuseScore y luego exportarla como MusicXML. Abrir el archivo .musicxml con un editor de texto (VS Code, Sublime Text, o incluso Bloc de Notas). Buscar etiquetas como `<note>`, `<dynamics>`, `<slur>` y modificarlas manualmente (cambiar un `mf` por `ff`, cambiar una negra por una corchea). Reimportar el archivo modificado en MuseScore y ver el resultado. Es un ejercicio de "cirugía XML" que revela cómo está construido internamente el formato.

---

*Guía docente — Tecnología Musical I | Sesión 24*
