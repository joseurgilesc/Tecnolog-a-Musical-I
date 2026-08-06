# Guía Docente — Sesión 28: Preparación de partes (particellas)

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivos `ejercicio_S28_partitura.mscz` (partitura general con 6+ instrumentos), `ejercicio_S28_particellas_sucias.mscz` (partes con errores para diagnosticar)  
**Referencia:** MuseScore Studio Handbook — Advanced topics: Parts

---

## Objetivo de la sesión

Que el estudiante domine el flujo completo de preparación de particellas profesionales: generación automática desde la partitura general, formateo específico para cada instrumento (tamaño de pentagrama, saltos de página, pausas multi-compás), inserción de cues para entradas guiadas, verificación de transposición en instrumentos transpositores, y exportación de partes listas para el atril. El estudiante debe internalizar que "generar partes" es un botón, pero "preparar partes" es un oficio.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S27 + pregunta disparadora: ¿quién lee las partes que generás? |
| **Desarrollo** | 30 min | Demostración: generación → diagnóstico → curaduría → cues → transposición → publicación |
| **Práctica** | 65 min | Generar partes, diagnosticar errores, corregir, insertar cues, exportar todo como PDF |
| **Cierre** | 15 min | Puesta en común del checklist de partes, reflexión, entrega |

---

## 1. Apertura — El músico en el atril

### Materiales
- Proyector con MuseScore Studio abierto.
- Archivo `ejercicio_S28_partitura.mscz` publicado en Classroom **antes de la clase**.
- Opcional: una parte profesional impresa de una orquesta real para mostrar como referencia.

### Dinámica

1. **Revisión de S27** (4 min):
   - ¿Cuál fue el mayor problema al preparar el layout de página? ¿Margenes? ¿Espaciado?
   - ¿Alguien descubrió algo que no esperaba sobre cómo se ve una partitura profesional?

2. **Preguntas disparadoras** (6 min):
   - Mostrar en proyector una partitura general de 8 pentagramas. Luego, mostrar SOLO la parte del clarinete generada automáticamente.
   - "¿Ven la diferencia de TAMAÑO entre la partitura general y la parte individual? ¿Por qué creen que el pentagrama de la parte es más grande?"
   - Respuesta esperada: "Porque el músico lee a distancia, desde el atril."
   - "Correcto. Pero no es solo el tamaño. Miren esta parte." Mostrar una parte con un salto de página en medio de un pasaje de semicorcheas. "¿Qué pasa si el clarinetista tiene que voltear la página AQUÍ?"
   - "Se cae la parte, se pierde, entra tarde." → "Exacto. Una parte mal formateada puede arruinar un concierto ENTERO."
   - **Frase para el pizarrón**: "El botón 'Generar partes' tarda 1 segundo. Preparar partes profesionales tarda 1 hora. La diferencia se nota en el primer ensayo."

---

## 2. Desarrollo — De partitura general a parte profesional

### Secuencia sugerida

1. **Generación automática: lo que MuseScore hace y lo que NO hace** (5 min). Con `ejercicio_S28_partitura.mscz`:
   - Archivo → Partes → Generar todas las partes.
   - "MuseScore acaba de crear una parte por cada instrumento. Veamos qué incluyó y qué NO."
   - Abrir la parte de Flauta I: "Vean: las notas están. Las dinámicas están. Las marcas de ensayo están."
   - "¿Qué FALTA?" Señalar:
     - El pentagrama tiene el mismo tamaño que la partitura general (5 mm → debe ser 7.5 mm).
     - Los saltos de página son los mismos que la partitura general (no tienen sentido para una parte individual).
     - No hay pausas multi-compás agrupadas.
     - No hay cues para entradas después de silencios largos.
   - "MuseScore GENERA las partes. Pero no las FORMATEA. El formateo es 100% tu responsabilidad."

2. **El checklist de curaduría de partes** (10 min). Para cada parte generada, revisar en este orden:
   
   **(a) Tamaño de pentagrama.** Formato → Estilo → Tamaño: 7.5 mm. "Es lo primero que hacés, ANTES de tocar cualquier otra cosa. Si ajustás saltos de página con pentagrama chico y después lo agrandás, todos los saltos se rompen."

   **(b) Saltos de página estratégicos.** "Esta es la parte más importante y la que más tiempo toma."
   - Activar vista "Diseño de página" (modo página continuo).
   - Regla de oro: "Cada salto de página debe ocurrir donde el músico tenga AL MENOS 2 segundos de silencio para voltear."
   - Mostrar cómo identificar silencios en la parte y colocar el salto de página JUSTO ANTES del silencio más largo.
   - "Si el músico está tocando semicorcheas sin parar durante 3 páginas, BUSCÁ una negra o blanca donde pueda respirar. Si no hay NINGÚN silencio, poné el salto donde haya una nota larga (blanca o redonda) y el músico pueda voltear con una mano."

   **(c) Pausas multi-compás.** "Si la flauta no toca durante 18 compases, NO escribimos 18 compases de silencio. Usamos UN bloque con el número."
   - Formato → Estilo → Pausas → Pausas multi-compás.
   - Mostrar la diferencia visual: 18 compases individuales vs. un bloque "18".
   - "Configurar el umbral: yo recomiendo agrupar a partir de 2 compases. Algunos editores usan 3. Lo importante es que sea CONSISTENTE en todas las partes."

   **(d) Cues (entradas guía).** "Durante silencios largos (+8 compases), el músico pierde la noción de dónde está. Necesita una GUÍA."
   - Mostrar cómo copiar una frase melódica de otro instrumento (ej. la melodía del oboe) y pegarla en la parte del clarinete durante su silencio.
   - Reducir el tamaño de las notas del cue a 60-70% (seleccionar → Propiedades → Tamaño de nota).
   - Agregar el nombre del instrumento que está tocando: "Ob." en texto pequeño sobre el cue.
   - "El cue NO se imprime en la partitura general. Solo existe en la parte individual."

   **(e) Números de compás y marcas de ensayo.**
   - Verificar que los números de compás aparezcan al inicio de cada sistema.
   - Verificar que las marcas de ensayo (A, B, C...) estén sincronizadas con la partitura general.
   - "Si el director dice 'vamos desde la letra D', TODOS los músicos deben encontrar la letra D en su parte. Si no está, el ensayo se detiene y 30 personas te miran feo."

   **(f) Transposición.** Para instrumentos transpositores:
   - Verificar que la parte esté en TONO ESCRITO (no de concierto). El botón de "tono de concierto" en la parte debe estar DESACTIVADO.
   - "El clarinetista en Si♭ lee su parte en Do Mayor aunque la obra esté en Si♭ Mayor. Si le das la parte en tono de concierto, va a tocar todo un tono DESAFINADO."

3. **Partes combinadas (merged parts)** (5 min):
   - "A veces dos instrumentos de la misma familia comparten una sola parte. Ejemplo: Flauta I y Flauta II en la MISMA hoja."
   - Cómo crear una parte combinada: Archivo → Partes → Nueva → seleccionar Flauta I y Flauta II → Crear.
   - "Esto se usa en orquestas escolares o ensambles chicos para ahorrar papel. Pero en contextos profesionales, cada músico recibe SOLO su línea."

4. **El nombre del instrumento y los metadatos** (5 min):
   - En partes profesionales, el nombre del instrumento aparece en CADA página (por si las hojas se mezclan en el atril).
   - Estilo → Cabecera y pie de página → agregar "Nombre de instrumento" al encabezado.
   - "También asegurate de que el número de página esté visible. Si se caen las hojas al suelo, el músico debe poder reordenarlas."

5. **Exportación masiva de partes** (5 min):
   - Archivo → Exportar → Exportar partes.
   - Seleccionar todas las partes → elegir PDF → seleccionar carpeta de destino.
   - "MuseScore exporta TODAS las partes en un solo paso. Pero antes de exportar, REVISASTE cada una individualmente, ¿verdad? ¿VERDAD?"

---

## 3. Práctica — El taller de particellas

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S28 — Preparación de partes (particellas)

**Material**: el docente proporciona dos archivos:

1. **`ejercicio_S28_partitura.mscz`**: Partitura general para 8 instrumentos: Flauta, Oboe, Clarinete en Si♭, Fagot, Trompa en Fa, Violín I, Violín II, Violonchelo. En Fa mayor (1 bemol), 4/4, 48 compases. La partitura debe estar musicalmente completa (todos los instrumentos tienen material durante al menos el 70% de la obra, con secciones de silencio variables). Las partes NO deben estar generadas todavía. Incluir marcas de ensayo (A–F) y dinámicas. Los pentagramas deben tener el tamaño estándar de partitura general (5.5 mm).

2. **`ejercicio_S28_particellas_sucias.mscz`**: Partitura para quinteto de vientos (Flauta, Oboe, Clarinete en Si♭, Trompa en Fa, Fagot) en Sol menor (2 bemoles), 3/4, 40 compases, con las partes YA generadas automáticamente pero con errores deliberados:
   - (a) Las partes tienen el tamaño de pentagrama de la partitura general (5.5 mm).
   - (b) Los saltos de página caen en medio de pasajes activos en al menos 3 de las 5 partes.
   - (c) No hay pausas multi-compás (todos los silencios son individuales).
   - (d) No hay cues en silencios de más de 12 compases.
   - (e) Las marcas de ensayo no son visibles en al menos 2 partes.
   - (f) La parte del clarinete está en tono de concierto (debería estar en tono escrito).
   - (g) Los nombres de instrumento no aparecen en todas las páginas.

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Generar las 8 partes desde la partitura general y formatearlas profesionalmente.
2. Diagnosticar y corregir los errores en las 5 partes del quinteto de vientos.
3. Insertar cues donde corresponda en ambas partituras.
4. Exportar todas las partes como PDFs individuales.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Generación de partes (8 instrumentos) | 8 partes generadas y abiertas; todas con pentagrama 7.5 mm | 6–7 partes correctas | ≤5 partes o sin cambio de tamaño |
| Saltos de página | Todos los saltos en silencios o notas largas (>2 s para voltear) en AMBAS partituras | Mayoría correcta pero 1–2 saltos mal ubicados | Múltiples saltos en pasajes activos |
| Pausas multi-compás | Configuradas en todas las partes; umbral consistente (2–3 compases) | Configuradas pero umbral inconsistente | Sin pausas multi-compás |
| Transposición | Partes de Clarinete y Trompa en tono escrito (botón de concierto DESACTIVADO) | Solo un instrumento correcto | Ambos incorrectos |
| Cues | Inserts visibles con nombre de instrumento en silencios ≥8 compases | Cues presentes pero sin nombre o en silencios cortos | Sin cues |
| Marcas y números | Marcas de ensayo y números de compás visibles en todas las partes | Faltan en 1–2 partes | Ausentes en ≥3 partes |
| Diagnóstico (quinteto) | ≥6 errores identificados y corregidos en el quinteto | 4–5 errores corregidos | ≤3 errores corregidos |
| Exportación | Todas las partes exportadas como PDF individuales con nombre de instrumento | Mayoría exportada correctamente | Archivos mal nombrados o incompletos |

---

## 4. Cierre — El oficio invisible

### Revisión por parejas (8 min)

- Intercambiar la parte de Flauta (partitura de 8): "¿Podrías tocar esta parte en un atril sin perderte? ¿Los saltos de página tienen sentido? ¿Las pausas multi-compás están claras?"
- Intercambiar el diagnóstico del quinteto: "¿Cuántos errores encontró tu compañero que vos no viste? ¿Cuáles?"

### Puesta en común (7 min)

- "Levanten la mano los que encontraron que corregir TODAS las partes tomó MÁS tiempo que el resto del ejercicio. ¿Cuánto tiempo les llevó?" (Estadística.)
- "¿Cuál fue el error más difícil de detectar en las partes sucias?" (Generalmente la transposición — es sutil si no sabés qué buscar.)
- "¿Qué parte fue la más difícil de formatear y por qué?" (Discusión sobre instrumentos con muchos silencios vs. instrumentos que tocan sin parar.)
- "¿Alguien tuvo que REHACER los saltos de página después de cambiar el tamaño de pentagrama?" → "ESA es la lección más importante de hoy: el orden IMPORTA. Primero tamaño, DESPUÉS saltos."

### Resumen del docente (5 min)

1. **"Generar partes" ≠ "Preparar partes".** El botón hace el 20% del trabajo. El 80% restante (formateo, saltos, cues, transposición, metadatos) es trabajo HUMANO. Ningún software hace esto automáticamente bien.

2. **El tamaño del pentagrama es lo primero.** Siempre. Sin excepciones. Si lo cambiás después, todos los saltos de página que pusiste se rompen y tenés que empezar de nuevo.

3. **Los saltos de página son la habilidad más subestimada del editor de partituras.** Un salto mal puesto puede arruinar un concierto. Un salto bien puesto pasa desapercibido. Paradójicamente, cuanto MEJOR es tu trabajo, MENOS se nota.

4. **Los cues salvan ensayos.** Un músico que pasó 34 compases en silencio necesita saber CUÁNDO entrar. Si no hay cue, va a contar compases (y probablemente se equivoque). Si hay cue, entra seguro. La diferencia es un ensayo fluido vs. un ensayo frustrante.

5. **El checklist es tu amigo.** Tamaño → Saltos → Pausas → Cues → Marcas → Transposición → Metadatos. Seguilo en orden. Siempre. Cuando estés cansado, el checklist piensa por vos.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| Los saltos de página se "rompen" al cambiar el tamaño del pentagrama | Es comportamiento esperado. El orden correcto es: (1) cambiar tamaño de pentagrama, (2) insertar saltos de página. Si ya pusiste los saltos antes de cambiar el tamaño, tendrás que rehacerlos. |
| Las pausas multi-compás no se agrupan automáticamente | Verificar en Formato → Estilo → Pausas que "Crear pausas multi-compás" esté activado. También verificar el umbral: si está en 4 compases pero el silencio es de 3, no se agrupará. Bajá el umbral a 2. |
| Los cues eran notas copiadas de otro pentagrama pero suenan en la reproducción | Seleccionar las notas del cue → Propiedades → marcar "Notas pequeñas" (small notes) y "Excluir de la reproducción". O mutearlas manualmente en el mezclador si es necesario. |
| La parte muestra el nombre del pentagrama como "Pista 1" en lugar de "Flauta" | Clic derecho en el pentagrama → Propiedades del pentagrama → cambiar "Nombre largo del instrumento" y "Nombre corto del instrumento". El nombre DEBE coincidir con el instrumento real. |
| El estudiante no identifica que la parte está en tono de concierto en lugar de tono escrito | Preguntar: "¿El clarinete en Si♭ lee en Do o transporta?" Si la respuesta es "transporta", preguntar: "¿Tu parte está transportada?" Enseñar a verificar: comparar la armadura de la parte de clarinete con la de flauta. Si son iguales y el clarinete está en Si♭, algo está mal (el clarinete debería tener 2 sostenidos MÁS o 2 bemoles MENOS). |
| Al exportar las partes como PDF, los nombres de archivo son genéricos ("Parte 1.pdf") | En el diálogo de exportación de partes, MuseScore usa por defecto el nombre de la parte como nombre de archivo. Si el estudiante renombró las partes en el diálogo de Partes, los PDFs heredarán esos nombres. Si no, enséñale a renombrar las partes primero. |
| La parte del fagot tiene todos los compases llenos y es imposible poner saltos de página en silencios | Si la parte NO tiene silencios, buscar compases con notas largas (blancas o redondas). Si no hay, buscar pasajes con negras en tempo lento. Si sigue sin haber pausas, usar la última nota de una frase como punto de giro (aunque no sea ideal). En música de cámara profesional, a veces no hay buena solución: se usan atriles dobles o tablets. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Parts](https://handbook.musescore.org/advanced-topics/parts.md)
- [MuseScore Studio Handbook — Staff/Part properties](https://handbook.musescore.org/advanced-topics/staff-part-properties.md)
- **Preparación del archivo `ejercicio_S28_partitura.mscz`**: crear partitura para 8 instrumentos en Fa mayor, 4/4, 48 compases. Cada instrumento debe tener material musical sustancial pero con secciones de silencio variables (Flauta toca en 38 compases, Fagot en 32, Violonchelo en 44, etc.). Incluir marcas de ensayo (A–F cada 8 compases), dinámicas, articulaciones. Los pentagramas deben ser de 5.5 mm (tamaño partitura general). NO generar las partes. La partitura debe tener suficiente material para que cada parte tenga al menos 2 páginas cuando se amplíe a 7.5 mm.
- **Preparación del archivo `ejercicio_S28_particellas_sucias.mscz`**: crear quinteto de vientos en Sol menor, 3/4, 40 compases. Escribir la obra completa. Luego generar las partes automáticamente y guardar el archivo. Reabrir e introducir los errores deliberados: no cambiar el tamaño de pentagrama, poner saltos de página en lugares pésimos (en medio de frases de semicorcheas), desactivar pausas multi-compás, no poner cues, ocultar marcas de ensayo en algunas partes, y dejar el clarinete en tono de concierto.
- Dato curioso: en el siglo XIX, los copistas profesionales de las editoriales de música (Ricordi, Breitkopf & Härtel, Durand) tenían reglas ESTRICTÍSIMAS sobre cómo debían formatearse las partes. Un copista podía ser despedido si una parte tenía un salto de página en un lugar incómodo. El oficio del copista era tan respetado como el del grabador o el impresor.
- Dato curioso: la invención de la tablet (iPad con ForScore o similar) está cambiando la forma en que los músicos leen partes: ya no hay que voltear páginas físicas. Pero IRÓNICAMENTE, muchas orquestas siguen usando papel porque: (1) es más barato que comprar 80 tablets, (2) no se queda sin batería en medio del concierto, (3) no se rompe si se cae del atril. El papel tiene futuro.
- Ejercicio opcional de ampliación: tomar una parte generada automáticamente y compararla con una parte equivalente de una edición profesional (Henle, Bärenreiter, Peters — disponibles en IMSLP). Identificar al menos 10 diferencias de formato entre la parte generada por software y la parte publicada profesionalmente. Esto desarrolla el "ojo editorial".

---

*Guía docente — Tecnología Musical I | Sesión 28*
