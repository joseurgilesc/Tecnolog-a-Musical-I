# Guía Docente — Sesión 6: Compases, métrica y operaciones de compás

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivo `ejercicio_S06_metrica.mscz` preparado por el docente  
**Referencia:** MuseScore Studio Handbook — Time signatures, Barlines, Measure operations, Measure numbering, Pickup and non-metered measures

---

## Objetivo de la sesión

Que el estudiante realice operaciones de compás con precisión (añadir, insertar, eliminar, duplicar), configure compases de anacrusa y compases con duración irregular, aplique cambios de indicación de compás entre métricas simples y compuestas, inserte barras divisorias simples, dobles y finales, y configure la numeración de compases excluyendo anacrusas y manteniendo numeración continua en cambios métricos.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S05 + activación con pregunta sobre estructura métrica |
| **Desarrollo** | 25 min | Demostración: añadir/insertar compases, anacrusa, cambio de compás, barras, numeración |
| **Práctica** | 70 min | Auditoría y corrección estructural + anacrusa + inserción de sección + cambio a 6/8 + barras + numeración |
| **Cierre** | 15 min | Revisión por parejas, puesta en común, entrega |

---

## 1. Apertura — Revisión y activación

### Materiales
- Proyector con MuseScore Studio abierto y una partitura de ejemplo de 16 compases en 4/4.
- El archivo `ejercicio_S06_metrica.mscz` publicado en Classroom **antes de la clase**.

### Dinámica

1. **Revisión rápida de S05** (5 min):
   - ¿Cuántos lograron detectar los 10 errores del ejercicio?
   - ¿Qué herramienta de edición les resultó más útil: Re-pitch, `J` para enarmonía o la transposición?
   - ¿Alguien usó el filtro de selección? ¿Para qué?

2. **Preguntas disparadoras** (5 min):
   - Proyectar una partitura simple de 8 compases en 4/4 y preguntar: "Si necesito meter una introducción de 4 compases antes de esta música, ¿qué hago? ¿Empiezo de nuevo?"
   - Reproducir un fragmento en 4/4 y hacer un cambio brusco a 6/8. Preguntar: "¿Qué cambió? ¿Por qué la música de repente 'baila' diferente?"
   - Mostrar un compás con anacrusa y preguntar: "¿Por qué este compás está incompleto? ¿Es un error o es a propósito?"

---

## 2. Desarrollo — Teoría guiada

### Secuencia sugerida

1. **Añadir, insertar y eliminar compases** (6 min). Sobre una partitura proyectada:
   - Seleccionar el último compás → `Ctrl + B`. Mostrar que se añade uno nuevo al final.
   - Seleccionar c.5 → `Ins`. Mostrar cómo UN compás vacío se inserta y todo el contenido desde c.5 se desplaza a la derecha.
   - `Ctrl + Z` para deshacer. Luego `Ctrl + Ins` → 3. Insertar 3 compases a la vez.
   - Seleccionar c.8 → `Ctrl + Supr`. Mostrar que el compás DESAPARECE. Los compases 9+ ahora empiezan una posición antes.
   - **Error deliberado**: seleccionar un compás y presionar SOLO `Supr` (sin `Ctrl`). Mostrar que el compás se vacía pero no desaparece. Preguntar: "¿Qué pasó? ¿Es esto lo que querían?"

2. **Anacrusa y compases incompletos** (5 min). Sobre el mismo archivo:
   - Clic derecho en el primer compás → **Propiedades del compás**. Modificar la duración **Real** a 1/8 (una corchea en 4/4). Mostrar cómo el compás se acorta.
   - Preguntar: "¿Qué número de compás debería tener este compás?" (Respuesta correcta: ninguno — la anacrusa no se numera.)
   - Marcar **Excluir del conteo de compases**. Mostrar que ahora el compás 1 es el primer compás completo.
   - Ir al último compás y mostrar cómo su duración también se puede ajustar para compensar la anacrusa.

3. **Indicaciones de compás simples y compuestas** (5 min). Sobre una partitura limpia:
   - Mostrar la paleta de Indicaciones de compás.
   - Insertar 4/4 en los primeros compases, luego seleccionar el compás 9 y elegir 6/8 en la paleta.
   - Explicar el re-agrupamiento automático: "MuseScore recalcula dónde cae cada nota según la nueva métrica."
   - Mostrar la diferencia entre 3/4 (ternario simple: 3 pulsos de negra) y 6/8 (binario compuesto: 2 pulsos de negra con puntillo). Hacer que los estudiantes palmeen ambos ritmos.

4. **Barras divisorias** (5 min). Sobre la partitura con cambio de compás:
   - Seleccionar la barra justo antes del cambio a 6/8.
   - Ir a la paleta **Líneas divisorias** y elegir **Doble barra**.
   - Ir al final y aplicar **Barra final**.
   - Mostrar el atajo con `Ctrl`: mantener `Ctrl` + clic en la barra de la paleta para aplicar solo a un pentagrama (barra local).
   - Preguntar: "¿Qué diferencia musical hay entre una barra simple y una doble?" (La doble señala un cambio estructural: nueva sección, nueva tonalidad, nueva métrica.)

5. **Numeración de compases** (4 min):
   - Ir a **Formato → Estilo → Numeración de compases**.
   - Activar **Mostrar numeración de compases**. Elegir "Al inicio de cada sistema".
   - Volver a la anacrusa: mostrar cómo ahora los números comienzan en el compás 2 (el primer compás completo).
   - Si el score tiene un salto de sección, mostrar cómo se reinicia la numeración y cómo desactivarlo desde **Propiedades** del salto de sección.

---

## 3. Práctica — Auditoría y reestructuración métrica

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S06 — Estructura métrica y operaciones de compás

**Material**: el docente proporciona el archivo `ejercicio_S06_metrica.mscz`, una partitura para flauta de 24 compases en 4/4, con los siguientes problemas estructurales (no revelar esta lista a los estudiantes; solo darles el archivo):

| Problema | Compás(es) | Descripción |
|---|---|---|
| Compás incompleto (sobra) | c. 3 | 4.5 tiempos. Hay una corchea de más. |
| Compás incompleto (falta) | c. 8 | 3.5 tiempos. Falta una corchea. |
| Compás vacío (error de `Supr`) | c. 15 | Contenido borrado pero el compás sigue ahí lleno de silencios. |
| Sin anacrusa pero la melodía lo necesita | c. 1 | La melodía arranca en el cuarto pulso; debería ser una anacrusa de negra. |
| Material desplazado | c. 18–24 | Las últimas notas deberían estar al final pero hay compases vacíos en el medio porque alguien eliminó con `Supr` en vez de `Ctrl + Supr`. |

También incluir indicaciones de que los compases 13 a 16 contienen una melodía en 4/4 que el estudiante deberá modificar y los compases 21 a 24 están en blanco.

**Preparación del archivo**: crear una melodía diatónica en Do mayor, 4/4, 24 compases. Insertar los problemas en los compases indicados. La anacrusa debe ser evidente: la melodía comienza en el cuarto pulso del compás 1 pero el compás está completo (4/4). Los compases 17 a 20 deben contener una sección melódica distinta.

**Instrucciones:**

Las mismas que en el `index.md` del estudiante (ver detalle en esa guía). En resumen:
1. Auditoría de compases (detección de problemas).
2. Corrección estructural (insertar/eliminar/ajustar duración).
3. Crear anacrusa y verificar cierre.
4. Insertar 4 compases nuevos con melodía original.
5. Cambio de compás a 6/8 a partir del compás 17.
6. Doble barra antes del cambio métrico + barra final.
7. Configurar numeración de compases.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Corrección estructural | La partitura tiene 24 compases correctos; no hay compases incompletos ni vacíos no previstos | 1–2 compases aún con problemas | ≥3 compases con errores estructurales |
| Anacrusa y cierre | La anacrusa dura una negra; el último compás se compensó; la numeración excluye la anacrusa | La anacrusa se creó pero el cierre no se ajustó | No realizó la anacrusa |
| Inserción y nueva sección | Insertó 4 compases en la posición correcta; la melodía nueva tiene coherencia melódica | Insertó los compases pero la melodía es incoherente | No insertó los compases |
| Cambio a 6/8 | El cambio está en la posición correcta; los compases en 6/8 cuadran rítmicamente con la nueva métrica | El cambio existe pero algunos compases no cuadran con 6/8 | No realizó el cambio |
| Barras divisorias | Doble barra antes del cambio métrico; barra final al terminar | Solo una de las dos barras está presente | No agregó barras divisorias |
| Numeración | Anacrusa excluida; números visibles en cada sistema; numeración continua | Falta uno de los tres criterios | No configuró la numeración |

---

## 4. Cierre — Estructura y organización

### Revisión por parejas (8 min)

Cada estudiante intercambia su archivo con un compañero:
- El compañero reproduce la partitura y verifica que cada compás suene completo (ni se corta antes ni se alarga).
- El compañero cuenta los compases: ¿hay exactamente 24? ¿Los compases insertados están donde deberían?
- El compañero revisa que la doble barra y la barra final estén visibles en el PDF.

### Puesta en común (7 min)

Preguntas para guiar la discusión:
- "¿Cuál fue el error más difícil de detectar: el compás incompleto o el compás vacío por `Supr`?" (Esperado: el vacío por `Supr`, porque la partitura se ve normal pero hay compases llenos de silencio que no deberían estar.)
- "Cuando insertan compases con `Ins`, ¿qué pasa con el contenido que ya estaba escrito?" (Se desplaza a la derecha.)
- "¿Qué diferencia notaron entre 4/4 y 6/8 al escribir? ¿Cómo cambió la sensación rítmica?"
- "Si tuvieran que explicarle a un compañero que faltó a clase cuándo usar `Supr` y cuándo `Ctrl + Supr`, ¿qué le dirían?"

### Resumen del docente (5 min)

1. Las operaciones de compás no son un detalle menor: **son la estructura del edificio**. Un compás mal insertado o mal eliminado desordena todo lo que viene después.
2. `Supr` borra contenido; `Ctrl + Supr` borra el compás entero. Si te equivocás, `Ctrl + Z` es tu mejor amigo.
3. La anacrusa no es un "error de compás": es una convención musical con reglas claras. El compás inicial se acorta y el último se compensa. La numeración empieza en el primer compás completo.
4. Los cambios de compás y las barras dobles comunican estructura al intérprete. Si la música cambia de 4/4 a 6/8 y no ponés doble barra, el intérprete puede no notar el cambio a tiempo.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| El estudiante usa `Supr` para eliminar un compás y se sorprende de que el compás sigue ahí | Mostrar la diferencia en vivo: `Supr` vs. `Ctrl + Supr`. Hacer que practiquen ambas en un compás de prueba. Es la confusión más frecuente de esta sesión. |
| Al insertar compases (`Ins`), el estudiante no entiende por qué la música se movió | Explicar que "insertar" es como abrir espacio en una fila: los que están detrás se corren. Si quería añadir al final, debía usar `Ctrl + B`. |
| La anacrusa no se ve reflejada en la numeración | Verificar que esté marcado **Excluir del conteo de compases** en las propiedades del compás. Si no, el número 1 aparecerá en la anacrusa. |
| Al cambiar a 6/8, las notas "desaparecen" o se desordenan | MuseScore re-agrupa los compases al cambiar la métrica. Algunas notas pueden perderse. Recomendar: siempre hacer el cambio de compás antes de escribir la música en esa sección. Con `Ctrl + Z` se puede deshacer si algo sale mal. |
| El estudiante intenta eliminar la armadura del primer compás y no puede | MuseScore no permite eliminar la armadura inicial (no sabe si querés Do mayor o atonal). En lugar de eliminar, debe seleccionar Do mayor de la paleta. |
| La barra final no se ve en el PDF porque quedó al final de un sistema sin compás siguiente | La barra final debe aplicarse al ÚLTIMO compás, no después. Si se insertó un compás vacío al final sin querer, eliminarlo con `Ctrl + Supr`. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Time signatures](https://handbook.musescore.org/notation/rhythm-meter-and-measures/time-signatures.md)
- [MuseScore Studio Handbook — Barlines](https://handbook.musescore.org/notation/rhythm-meter-and-measures/barlines.md)
- [MuseScore Studio Handbook — Measure properties](https://handbook.musescore.org/notation/rhythm-meter-and-measures/measure-properties.md)
- [MuseScore Studio Handbook — Measure numbering](https://handbook.musescore.org/notation/rhythm-meter-and-measures/measure-numbering.md)
- [MuseScore Studio Handbook — Pickup and non-metered measures](https://handbook.musescore.org/notation/rhythm-meter-and-measures/pickup-and-non-metered-measures.md)
- [MuseScore Studio Handbook — Adding and removing measures](https://handbook.musescore.org/basics/adding-and-removing-measures.md)
- **Preparación del archivo de ejercicio** (`ejercicio_S06_metrica.mscz`): crear partitura para flauta en Do mayor, 4/4, 24 compases. Insertar los problemas descritos en la sección de práctica. La melodía debe ser diatónica y cantable para facilitar la detección auditiva.
- Dato para compartir: la diferencia entre `Ins` y `Ctrl + B` es una de las preguntas más frecuentes en los foros de MuseScore. Muchos usuarios novatos insertan cuando quieren añadir y viceversa. La regla: `Ins` para el medio, `Ctrl + B` para el final.

---

*Guía docente — Tecnología Musical I | Sesión 6*
