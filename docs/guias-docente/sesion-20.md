# Guía Docente — Sesión 20: Transposición y escritura para instrumentos transpositores

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivos `ejercicio_S20_transporte.mscz`, `ejercicio_S20_armadura.mscz` y `ejercicio_S20_banda.mscz` preparados por el docente  
**Referencia:** MuseScore Studio Handbook — Notation: Transposition, Concert pitch

---

## Objetivo de la sesión

Que el estudiante domine los tres mecanismos de transposición en MuseScore (cambio de tonalidad, configuración de instrumento, y toggle de tono de concierto), comprenda la diferencia conceptual entre tono escrito y tono de concierto, identifique correctamente la transposición de los instrumentos más comunes (Si♭, Mi♭, Fa, octava), corrija armaduras de key signature en partituras mal configuradas, y componga para ensambles con instrumentos transpositores alternando fluidamente entre las dos vistas.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S19 + pregunta disparadora: ¿por qué el clarinete toca una nota diferente a la que lee? |
| **Desarrollo** | 30 min | Demostración: tres formas de transponer → instrumentos transpositores uno por uno → checklist de armaduras |
| **Práctica** | 65 min | Transporte de tonalidad → armaduras de cuarteto → corrección de banda → cuarteto propio → banda de vientos |
| **Cierre** | 15 min | Revisión por parejas, puesta en común: el "baile de armaduras", entrega |

---

## 1. Apertura — El clarinete que toca "otra cosa"

### Materiales
- Proyector con MuseScore Studio abierto.
- Los archivos `ejercicio_S20_transporte.mscz`, `ejercicio_S20_armadura.mscz` y `ejercicio_S20_banda.mscz` publicados en Classroom **antes de la clase**.

### Dinámica

1. **Revisión rápida de S19** (5 min):
   - ¿Lograron que la tablatura y el pentagrama mostraran la misma melodía? ¿Ajustaron posiciones con Ctrl+↑/↓?
   - ¿El solo con bends, slides y hammer-ons sonó a guitarra o a piano MIDI?
   - ¿Los diagramas de trastes: abiertos o con cejilla? ¿Cuándo usar cada uno?
   - ¿La lead sheet final: las 4 capas de información (pentagrama, tab, cifrado, diagramas)?

2. **Preguntas disparadoras** (5 min):
   - Proyectar un Do central en el pentagrama. Preguntar: "Si un pianista toca este Do, suena Do. Si un clarinetista toca ESTE MISMO Do escrito, ¿qué suena?" (Si♭, un tono más bajo). "¿Por qué? ¿Está desafinado el clarinete? ¿Es un error de la partitura?"
   - "Levanten la mano: ¿quién toca o ha tocado un instrumento de viento? ¿Clarinete, saxofón, trompeta, trompa?" (Estadística rápida. Los que tocan estos instrumentos ya VIVEN la transposición; los que tocan piano o guitarra suelen no saber que existe.)
   - "Si yo compongo una melodía en Do Mayor para piano y quiero que el clarinete en Si♭ la toque, ¿en qué tonalidad debo escribir la parte del clarinete?" (Re Mayor, 2 sostenidos). Ver quién responde correctamente.
   - Mostrar la partitura general alternando tono de concierto y tono escrito. "¿Qué cambió? ¿Las notas? ¿Las armaduras? ¿Ambas?" (Solo las armaduras y la visualización; las notas suenan igual.)

---

## 2. Desarrollo — Las tres transposiciones de MuseScore

### Secuencia sugerida

1. **Transposición diatónica: cambiar la tonalidad de una pieza** (7 min). Proyectar `ejercicio_S20_transporte.mscz`:
   - "Tres formas de transponer en MuseScore. La primera y más obvia: cambiar la TONALIDAD de una pieza existente."
   - Seleccionar todo (`Ctrl + A`) → Herramientas → Transponer → A una tonalidad → elegir La Mayor. "Toda la pieza subió un tono. Las relaciones entre notas son las mismas. Es la MISMA melodía, solo que más aguda."
   - Mostrar la diferencia entre "Por intervalo" (movés X semitonos) y "A una tonalidad" (elegís la tonalidad destino). "¿Cuál usar? Si sabés la tonalidad de destino, usá 'A una tonalidad'. Si solo querés subir o bajar una cantidad fija, usá 'Por intervalo'."
   - **Advertencia**: "Si transponés una pieza de piano 2 octavas arriba, muchas notas van a sonar ridículas. Siempre verificá el rango del instrumento."
   - "¿Las alteraciones se ajustan automáticamente?" (Sí, MuseScore ajusta sostenidos y bemoles para mantener las relaciones diatónicas.)

2. **Transposición de instrumento: la configuración que NO se ve** (8 min). Proyectar una partitura con flauta y clarinete:
   - "Segunda forma: la transposición INHERENTE al instrumento. Esto NO es un comando que ejecutás. Es una propiedad que CONFIGURÁS."
   - Clic derecho en el pentagrama del clarinete → Propiedades del pentagrama → Transposición.
   - "Para clarinete en Si♭: 'Suena una 2ª mayor más bajo de lo escrito.' Esto significa: lo que el músico LEE está un tono POR ENCIMA de lo que SUENA."
   - "¿Por qué existe esto? Porque así el clarinetista usa la MISMA digitación para tocar en clarinete en Si♭, en La, en Mi♭... Lee Do, digita Do, y el instrumento produce la nota correcta para ese tamaño de tubo."
   - Mostrar el botón de tono de concierto. "Tercera 'forma': NO es una transposición. Es un INTERRUPTOR DE VISTA. Como cambiar el idioma de un menú. La comida es la misma, pero la ves en español o en inglés."
   - Activar/desactivar varias veces. "¿Ven? Las armaduras 'bailan'. El clarinete pasa de mostrar 3 bemoles (tono concierto) a 1 bemol (tono escrito). LAS NOTAS NO CAMBIARON."

3. **Los instrumentos transpositores uno por uno** (8 min). Tabla en el proyector:
   - **Familia Si♭**: Clarinete, trompeta, saxofón soprano, saxofón tenor. "Regla: armadura escrita = +2 sostenidos (o −2 bemoles) respecto a la de concierto."
   - **Familia Mi♭**: Saxofón alto, saxofón barítono, clarinete requinto. "Regla: +3 sostenidos."
   - **Familia Fa**: Trompa. "Regla: +1 sostenido. ¡NO se confundan! La trompa en Fa NO es como el clarinete en Si♭. Es SU PROPIA transposición."
   - **Transposición de octava**: Flautín (8ª arriba), guitarra (8ª abajo), contrabajo (8ª abajo), glockenspiel (15ª arriba).
   - **NO transpositores**: Flauta, oboe, fagot, trombón, tuba (en Do), violín, viola, cello, piano. "Estos instrumentos suenan EXACTAMENTE lo que leés."
   - **Pregunta trampa**: "El cello lee en clave de Fa. ¿Es transpositor?" (NO. La clave NO es transposición. El cello lee Do₃ en clave de Fa y suena Do₃. La transposición es cuando lo que suena NO coincide con lo escrito en la MISMA clave.)

4. **Checklist del compositor** (7 min). Proyectar la checklist:
   - "Componé SIEMPRE en tono de concierto. Imprimí SIEMPRE en tono escrito."
   - "Antes de escribir, hacé la tabla de armaduras de tus instrumentos."
   - "Verificá rangos: un clarinete no puede tocar Mi₂ de concierto. Suena Re₃ como nota más grave."
   - "Generá las partes individuales y revisalas UNA POR UNA. El clarinetista no debería ver 3 bemoles si la obra está en Mi♭ Mayor de concierto."
   - Mostrar el error más común: partitura general con todos los pentagramas mostrando la MISMA armadura (error en `ejercicio_S20_banda.mscz`). "Esto es un DESASTRE. El clarinete estaría leyendo en Mi♭ Mayor pero debería leer en Fa Mayor. El saxofón alto, en Re Mayor. Si imprimís esta partitura, el ensayo va a ser un caos."

---

## 3. Práctica — Transposición y escritura para instrumentos transpositores

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S20 — Transposición y escritura para instrumentos transpositores

**Material**: el docente proporciona tres archivos:

1. **`ejercicio_S20_transporte.mscz`**: Partitura para piano solo en Sol Mayor (1 sostenido), 4/4, 16 compases. Melodía diatónica en la mano derecha (Do₄–Sol₅) con ámbito de una octava y media, acompañamiento de acordes triádicos en la mano izquierda. La pieza debe ser diatónica, con algunas notas cromáticas de paso para que las alteraciones accidentales se pongan a prueba durante la transposición. Diseñada para que al transportar a Mi♭ Mayor y Mi Mayor algunas notas queden cerca pero no fuera del rango del piano (verificar previamente).

2. **`ejercicio_S20_armadura.mscz`**: Partitura para cuarteto de vientos: Flauta, Clarinete en Si♭, Trompa en Fa, Fagot. En Mi♭ Mayor (3 bemoles) de concierto, 4/4, 24 compases. Melodía simple en la flauta (negras y corcheas, ámbito Do₄–La₅). Notas largas (redondas y blancas) en clarinete, trompa y fagot formando acordes de la armonía de Mi♭ Mayor. IMPORTANTE: los instrumentos transpositores DEBEN estar configurados correctamente desde la plantilla para que el toggle de tono de concierto funcione. El estudiante verificará las armaduras en tono escrito.

3. **`ejercicio_S20_banda.mscz`**: Partitura para ensamble de vientos: Flauta, Clarinete en Si♭, Saxofón alto en Mi♭, Saxofón tenor en Si♭. En Fa Mayor (1 bemol) de concierto, 4/4, 20 compases. Melodía en tutti (todos al unísono/octavas). ERROR DELIBERADO: los pentagramas del clarinete, saxofón alto y saxofón tenor NO tienen configurada la transposición en Propiedades del pentagrama. Todos muestran Fa Mayor (1 bemol). El estudiante debe configurar la transposición de cada uno y verificar que, en tono escrito, muestren las armaduras correctas (Sol Mayor para Si♭, Re Mayor para Mi♭).

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Transponer la pieza de piano a 3 tonalidades diferentes.
2. Verificar y corregir armaduras en el cuarteto de vientos.
3. Diagnosticar y corregir la banda con transposición mal configurada.
4. Crear un cuarteto flauta/clarinete/violín/cello con melodía compartida transportada.
5. Componer para banda de 6 instrumentos con todas las transposiciones correctas.
6. Reflexionar sobre el concepto de transposición instrumental.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Transposición de tonalidad | 3 transportes correctos; notas en rango; armaduras aplicadas | 2 correctos | ≤1 correcto |
| Armaduras transpositoras | Clarinete y trompa con armaduras verificadas/corregidas; Staff Texts identificando cada una | Una correcta, otra no | Ninguna corregida |
| Corrección de banda | Cl, SaxA, SaxT con transposición configurada y armaduras correctas en tono escrito; partes exportadas | 2 de 3 instrumentos corregidos | ≤1 instrumento corregido |
| Cuarteto propio | Flauta + Clarinete al unísono (transporte correcto); Vl y Vc en Re Mayor; armaduras correctas | Errores en la transposición del clarinete | Clar no suena al unísono con flauta |
| Banda de vientos | 6 instrumentos bien configurados; composición en Si♭ Mayor; todas las armaduras correctas en tono escrito | 4–5 bien | ≤3 bien |
| Reflexión | 3 respuestas con comprensión conceptual; explica el "porqué" de los instrumentos transpositores | 2 correctas | ≤1 correcta |

---

## 4. Cierre — El baile de las armaduras

### Revisión por parejas (8 min)

- Intercambiar `ejercicio_S20_armadura_corregida.mscz`: "Activá y desactivá el tono de concierto. ¿Las armaduras del clarinete y la trompa son correctas? ¿El clarinete muestra 1 bemol en tono escrito? ¿La trompa muestra 2 bemoles?"
- Intercambiar `ejercicio_S20_banda_corregida.mscz`: "Abrí las partes individuales. ¿El clarinete tiene 1 sostenido (Sol Mayor)? ¿El saxofón alto tiene 2 sostenidos (Re Mayor)? Si no, está mal."
- Intercambiar el cuarteto propio: "Reproducilo. ¿La flauta y el clarinete suenan al unísono en los compases 1–8? Si no suenan igual, la transposición del clarinete está mal calculada."

### Puesta en común (7 min)

- "¿Por qué existen los instrumentos transpositores? La respuesta NO es 'porque sí' o 'por tradición'. Hay tres razones concretas: familias de instrumentos con misma digitación, tradición de las trompas naturales, y evitar líneas adicionales. ¿Alguien puede explicar la primera razón con el ejemplo del saxofonista que cambia de saxofón alto a tenor?"
- "¿En qué vista componemos: tono de concierto o tono escrito?" (Tono de concierto, SIEMPRE. Si componés en tono escrito, no tenés idea de qué están sonando realmente los instrumentos. Los acordes que ves no son los acordes que suenan.)
- Discusión: "¿El clarinete en Si♭ es un instrumento 'mal afinado' o 'defectuoso' porque su Do no es un Do real?" (NO. Es una CONVENCIÓN para facilitar la vida del instrumentista. El clarinete está perfectamente afinado... en Si♭. El Do escrito es un Si♭ real porque así el clarinetista puede usar la misma digitación en toda la familia de clarinetes.)

### Resumen del docente (5 min)

1. **Tres transposiciones en MuseScore, tres propósitos diferentes.** Cambio de tonalidad (movés la pieza), configuración de instrumento (definís cómo se interpreta), y toggle de vista (cambiás lo que ves sin modificar nada). No las confundan. 
2. **Componé en tono de concierto, imprimí en tono escrito.** Si no seguís esta regla, vas a escribir acordes que no existen y notas fuera de rango. El botón de tono de concierto es tu AMIGO.
3. **Los intervalos de transposición son fijos y predecibles.** Si♭ → +2♯, Mi♭ → +3♯, Fa → +1♯. No hay magia: es aritmética de armaduras.
4. **Una partitura bien transpuesta es invisible.** El músico no debería notar que hubo transposición. Lee su parte, toca sus notas, y todo suena como el compositor quiso. Si el músico pregunta "¿esto está bien?", algo falló en tu configuración.
5. **La transposición NO es un error ni una complicación innecesaria.** Es una HERRAMIENTA que resuelve problemas reales: unificar digitaciones entre instrumentos de la misma familia, respetar tradiciones históricas, y mantener la música legible en el pentagrama.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| El estudiante transpone la pieza de piano y las notas quedan fuera del teclado (ej. Mi♭₇ transportado 2 octavas arriba) | Recordar que la transposición de tonalidad no verifica rangos automáticamente. Después de transponer, revisar nota por nota que estén dentro del rango del instrumento. Si alguna nota quedó fuera, transportar por una octava diferente o ajustar el pasaje. |
| El estudiante confunde el toggle de tono de concierto con una transposición real | "Es un interruptor de VISTA, no un comando de transposición. Las notas del archivo no cambian. Solo cambia lo que ves. Como poner lentes de sol: el mundo no se oscurece, solo tu percepción." Mostrar que al guardar, cerrar y reabrir el archivo, el estado del toggle se mantiene como estaba. |
| Al configurar la transposición del clarinete, el estudiante pone "2ª mayor ascendente" en lugar de "descendente" y el clarinete suena más agudo en lugar de más grave | La dirección del intervalo es CRÍTICA. Para clarinete en Si♭: "suena una 2ª mayor más BAJO de lo escrito" = el tono de concierto es MENOR que el escrito. Si se configura al revés, el clarinete sonará una 2ª mayor más AGUDO. Verificar con el oído: el Do escrito del clarinete debe sonar como Si♭ de concierto, no como Re. |
| El estudiante no entiende por qué la armadura de la trompa es diferente a la del clarinete si ambas están en la misma pieza | "Porque cada familia tiene su PROPIA transposición. El clarinete en Si♭ transpone una 2ª mayor. La trompa en Fa transpone una 5ª justa. Como los intervalos son diferentes, las armaduras resultantes son diferentes. Es matemática, no magia." |
| El estudiante genera las partes y la parte del clarinete muestra la armadura de concierto en lugar de la escrita | Verificar que la transposición del instrumento esté configurada en Propiedades del pentagrama de la partitura GENERAL. Las partes heredan esta configuración. Si en la partitura general el clarinete no tiene transposición configurada, las partes tampoco la tendrán. |
| El estudiante escribe para saxofón alto en Mi♭ y se confunde: "¿qué nota escribo para que suene Do?" | Truco nemotécnico: "El saxofón alto está en Mi♭. Do escrito suena Mi♭ (una 6ª mayor abajo). Para que suene Do de concierto, tengo que escribir La (una 6ª mayor arriba de Do)." Hacer el ejercicio inverso: "Si quiero que el saxofón alto suene Sol₃ de concierto, ¿qué nota escribo?" (Mi₄ escrito). |
| La transposición de octava (flautín, guitarra, contrabajo) parece "más fácil" pero el estudiante la ignora | Recordar que la transposición de octava TAMBIÉN es transposición. Si escribís un Do₄ para flautín, suena Do₅. Si no lo sabés, tu orquestación va a sonar una octava desplazada. Verificá SIEMPRE en el manual qué transposición tiene cada instrumento antes de escribir para él. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Transposition](https://handbook.musescore.org/notation/transposition)
- [MuseScore Studio Handbook — Concert pitch](https://handbook.musescore.org/sound-and-playback/concert-pitch)
- **Preparación del archivo `ejercicio_S20_transporte.mscz`**: partitura para piano solo, Sol Mayor, 4/4, 16 compases. Melodía: Do₄–Sol₅, mayoritariamente diatónica con algunas notas cromáticas de paso (Fa♯, Do♯) para que la transposición ponga a prueba las alteraciones. Acompañamiento: acordes triádicos en bloque (redondas y blancas). Verificar que al transportar a Mi♭ Mayor y Mi Mayor las notas sigan dentro del teclado de 88 teclas.
- **Preparación del archivo `ejercicio_S20_armadura.mscz`**: cuarteto de vientos: Fl + Cl(Si♭) + Tpa(Fa) + Fg. Mi♭ Mayor (3 bemoles). Melodía simple en flauta (Do₄–La₅, negras y corcheas). Clarinete, trompa y fagot con notas largas (redondas y blancas) en acordes de Mi♭ Mayor (I, IV, V, vi). LOS INSTRUMENTOS DEBEN AGREGARSE DESDE LA PLANTILLA DE MUSEOSCORE (no desde "Instrumento genérico") para que la transposición esté preconfigurada. El estudiante solo debe VERIFICAR que las armaduras sean correctas en tono escrito.
- **Preparación del archivo `ejercicio_S20_banda.mscz`**: ensamble de vientos: Fl, Cl(Si♭), SaxA(Mi♭), SaxT(Si♭). Fa Mayor (1 bemol). Melodía en tutti (todos al unísono u octavas). ERROR DELIBERADO: agregar los instrumentos NO desde la plantilla sino como "Instrumento en Do" genérico. Luego, en Propiedades del pentagrama, NO configurar la transposición. El resultado: todos los pentagramas muestran 1 bemol. El estudiante debe configurar la transposición de Cl, SaxA y SaxT manualmente y verificar que las armaduras cambien correctamente en tono escrito.
- Dato curioso: la transposición en la música existe desde hace siglos. En el Renacimiento y Barroco, los instrumentos de viento (chirimías, cornetos, sacabuches) se construían en diferentes tamaños y cada tamaño tenía su propia "transposición natural". La práctica de escribir todo "como si fuera en Do" (transposición escrita) se estandarizó en el siglo XVIII.
- Dato curioso: en las bandas británicas de metales (brass bands), TODOS los instrumentos —excepto el trombón bajo— son transpositores y se leen en clave de Sol. La tuba en Si♭ lee en clave de Sol y transpone una 9ª mayor. Esto significa que un tubista de brass band lee las mismas notas que un trompetista, solo que suenan dos octavas más graves.
- Dato curioso: el saxofón fue inventado por Adolphe Sax en 1840 con la intención de crear una familia completa de instrumentos (sopranino al sub-contrabajo) que compartieran digitación. La transposición es una CARACTERÍSTICA DE DISEÑO, no un defecto. Sax concibió el saxofón como una familia transpositora desde el día uno.
- Ejercicio opcional de ampliación: entregar una partitura de una sinfonía clásica (Haydn o Mozart) en PDF y pedir a los estudiantes que identifiquen los instrumentos transpositores y deduzcan la tonalidad de concierto a partir de las armaduras escritas. Por ejemplo: "Si la parte de trompa en Fa tiene 1 bemol, ¿en qué tonalidad de concierto está la sinfonía?" (Si♭ Mayor, porque el +1♯ de la trompa cancela el bemol y da 2 bemoles en total). Esto entrena la lectura de partituras orquestales históricas.

---

*Guía docente — Tecnología Musical I | Sesión 20*
