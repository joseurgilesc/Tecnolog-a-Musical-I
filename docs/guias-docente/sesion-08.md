# Guía Docente — Sesión 8: Valores irregulares, puntillos y agrupación rítmica

**Duración estimada:** 1 sesión presencial (≈ 2 horas)  
**Herramientas:** MuseScore Studio 4, Google Classroom, proyector, archivo `ejercicio_S08_ritmo.mscz` preparado por el docente  
**Referencia:** MuseScore Studio Handbook — Tuplets, Beams; MuseScore 3 Handbook — Tuplets, Beams, Grace notes

---

## Objetivo de la sesión

Que el estudiante construya tresillos, quintillos, sextillos y valores irregulares anidados en distintos contextos métricos, ingrese notas con puntillo simple y doble verificando la completitud rítmica de cada compás, modifique el barrado de corcheas y semicorcheas tanto a nivel global (propiedades del compás) como local (propiedades de nota), e inserte notas de adorno (apoyaturas y acciaccaturas) comprendiendo la diferencia rítmica entre ambos tipos.

---

## Esquema de la clase

| Momento | Duración | Actividad |
|---|---|---|
| **Apertura** | 10 min | Revisión de S07 + activación con patrones rítmicos |
| **Desarrollo** | 25 min | Demostración: tresillos, quintillos, anidamiento, puntillos, barrado, notas de adorno |
| **Práctica** | 70 min | Construcción de tresillos → quintillo/sextillo → anidamiento → puntillos → barrado personalizado → notas de adorno |
| **Cierre** | 15 min | Revisión por parejas, escucha crítica colectiva, entrega |

---

## 1. Apertura — Revisión y activación

### Materiales
- Proyector con MuseScore Studio abierto.
- El archivo `ejercicio_S08_ritmo.mscz` publicado en Classroom **antes de la clase**.

### Dinámica

1. **Revisión rápida de S07** (5 min):
   - ¿Entendieron la diferencia entre alteración propia y accidental?
   - ¿Alguien tuvo problemas con la transposición? ¿Qué pasó con las alteraciones accidentales al transponer?
   - ¿Les sorprendió que el clarinete necesite otra armadura para sonar igual?

2. **Preguntas disparadoras** (5 min):
   - Proyectar un compás en 4/4 con tres corcheas agrupadas bajo un `3` y preguntar: "¿Cuánto dura este grupo? ¿Es justo o está 'trampeando' la métrica?"
   - Palmear un ritmo simple: "ta ta-ta ta". Luego palmear un tresillo sobre el mismo pulso: "ta-ki-ta ta". Preguntar: "¿Qué cambió en la subdivisión?"
   - Mostrar dos compases idénticos pero con barrado diferente (uno agrupado por pulsos, otro con barras continuas). Preguntar: "¿Cuál se lee más fácil? ¿Por qué?"
   - "¿Alguna vez vieron esas notas chiquitas antes de una nota normal? ¿Qué son y para qué sirven?"

---

## 2. Desarrollo — Teoría guiada

### Secuencia sugerida

1. **Tresillos y valores irregulares básicos** (6 min). Partitura limpia proyectada:
   - Explicar la regla de oro: **duración total primero, división después**.
   - Demostrar un tresillo de corcheas: `N` → `5` (negra, porque el tresillo de corcheas ocupa 1 tiempo) → `Ctrl + 3` → ingresar 3 notas.
   - Preguntar: "¿Por qué seleccioné `5` (negra) y no `4` (corchea)?" (Porque el tresillo de corcheas ocupa el espacio de UNA negra. La duración que elegís es la del GRUPO COMPLETO, no la de cada nota.)
   - Demostrar un tresillo de negras: `N` → `6` (blanca) → `Ctrl + 3` → ingresar 3 negras. Ocupa el espacio de una blanca.
   - Error deliberado: seleccionar `4` (corchea) y luego `Ctrl + 3`. Mostrar que el tresillo queda "microscópico" (3 fusas en espacio de corchea).
   - Mostrar los atajos `Ctrl + 2` a `Ctrl + 9`. Explicar que `Ctrl + 5` crea un quintillo y `Ctrl + 6` un sextillo, ambos sobre la duración seleccionada.

2. **Valores irregulares anidados** (4 min). Sobre un tresillo ya creado:
   - Seleccionar la primera corchea del tresillo.
   - `N` → `4` (corchea) → `Ctrl + 3`. Mostrar que ahora esa corchea se divide en 3 semicorcheas.
   - Explicar: "Es un tresillo dentro de otro. La cuenta total del compás sigue siendo correcta porque el tresillo exterior ocupa 1 tiempo y el interior ocupa ½ tiempo."
   - Mostrar el diálogo **Añadir → Grupos irregulares → Otro...** para crear valores personalizados (ej. 11:8).

3. **Puntillo simple y doble** (5 min). En modo ingreso:
   - Demostrar la secuencia: `N` → `5` → `.` → `C` (Do negra con puntillo).
   - Preguntar: "¿Cuánto dura? ¿Una negra y media, verdad? ¿Qué nota necesito después para completar el tiempo?" (Una corchea.)
   - Demostrar el error típico: escribir `N` → `5` → `C` → `.`. La nota ya se escribió sin puntillo. El `.` debe ir ANTES de la nota.
   - Doble puntillo: desde la paleta **Más → Figuras → Puntillos** o desde el panel **Propiedades** de la nota.
   - Preguntar: "¿Cuánto agrega el doble puntillo?" (La mitad + la mitad de la mitad = 3/4 del valor original.)

4. **Agrupación rítmica y barrado** (6 min). Sobre una partitura con abundantes corcheas y semicorcheas en 4/4:
   - Mostrar el barrado por defecto: corcheas agrupadas en pares (2+2+2+2), semicorcheas en bloques de 4 (4+4+4+4).
   - **Barrado global**: seleccionar la indicación de compás → **Propiedades de indicación de compás** → **Grupos de barras**. Hacer clic en el diagrama para modificar cómo se agrupan las notas en cada pulso. Aplicar a todo el score.
   - **Barrado local**: seleccionar una nota → pestaña **Barra** en **Propiedades**. Mostrar cada opción:
     - **Unir barras**: fuerza la unión con la nota anterior.
     - **Romper barra izquierda**: rompe la barra que viene de la nota anterior.
     - **Sin barra**: rompe todas las barras de esa nota.
   - **Barrado sobre silencio**: seleccionar un silencio entre dos corcheas → **Unir barras**. Mostrar que la barra "salta" sobre el silencio.
   - **Barrado sobre línea divisoria**: seleccionar la primera nota del compás siguiente → **Unir barras**. Mostrar cómo la barra cruza la barra de compás.

5. **Notas de adorno** (4 min). Sobre un pasaje ya escrito:
   - Seleccionar una negra → paleta **Notas de adorno** → **Apoyatura**. Ingresar la altura. Mostrar la nota pequeña sin tachar.
   - Seleccionar otra negra → **Acciaccatura**. Mostrar la nota pequeña con barra oblicua.
   - Reproducir ambas. Preguntar: "¿Notan la diferencia de duración? La apoyatura 'roba' más tiempo de la nota principal que la acciaccatura."
   - Mostrar cómo agregar varias notas de adorno consecutivas antes de una misma nota.

---

## 3. Práctica — Ritmo y agrupación

### Actividad en Classroom

Publicar como **Tarea** en Google Classroom:

**Título:** S08 — Valores irregulares y agrupación rítmica

**Material**: el docente proporciona el archivo `ejercicio_S08_ritmo.mscz`, una partitura para instrumento de teclado (piano, gran pentagrama) en Do mayor, 4/4, 24 compases.

**Preparación del archivo:**
- Compases 1 a 12: melodía en la mano derecha con figuras de negra, corchea, semicorchea, y algunos silencios. La mano izquierda puede tener un acompañamiento sencillo (blancas o redondas). El propósito de esta sección es que el estudiante transforme grupos de corcheas en tresillos y experimente con quintillos/sextillos.
- Compases 11 y 12: figuras con valores regulares (negras y corcheas) para que el estudiante pueda aplicar puntillos.
- Compases 13 a 20: vacíos. El estudiante creará aquí su propia melodía para practicar el barrado personalizado.
- Compases 21 a 24: vacíos (o con algunas notas largas). El estudiante insertará aquí las notas de adorno.

**Instrucciones:** según el detalle en el `index.md` del estudiante. En resumen:
1. Tresillos de corchea y de negra (c. 1–4).
2. Quintillo y sextillo de semicorchea (c. 5–8).
3. Tresillo anidado (c. 9).
4. Puntillos y doble puntillo (c. 11–12).
5. Melodía propia con barrado personalizado (c. 13–20).
6. Notas de adorno: apoyaturas y acciaccaturas (c. 21–24).
7. Escucha crítica y corrección de errores rítmicos.

### Rúbrica formativa

| Criterio | ✅ Logrado | ⚠️ En proceso | ❌ No logrado |
|---|---|---|---|
| Tresillos | Todos los tresillos cuadran; compases suman exactamente 4 tiempos; construidos con la duración correcta | 1–2 compases con error de duración | ≥3 compases con error |
| Quintillo y sextillo | Ambos correctamente construidos; diferencia auditiva perceptible | Uno correcto, otro incorrecto | No realizados |
| Tresillo anidado | Anidamiento correcto; compás cuadra | Anidamiento con error de duración | No realizado |
| Puntillos | Puntillos y doble puntillo correctos; compases cuadran | Puntillos correctos pero sin doble puntillo | Error rítmico grave |
| Barrado personalizado | Modificado en ≥3 compases; barra sobre silencio; resultado legible | Modificado pero poco legible o sin barra sobre silencio | No modificó |
| Notas de adorno | Dos apoyaturas y dos acciaccaturas; diferencia identificada | Un tipo presente, otro ausente | No insertadas |
| Escucha crítica | Detectó y corrigió errores rítmicos | Escuchó sin corregir | No revisó |

---

## 4. Cierre — Ritmo y precisión

### Revisión por parejas (8 min)

Cada estudiante intercambia archivos con un compañero:
- El compañero cuenta en voz alta mientras reproduce: verificando que los tresillos suenen uniformes.
- Verifica que los compases con puntillos no se "desborden" (no duren más de lo que deben).
- Revisa que las notas de adorno no hayan desplazado rítmicamente el resto del compás.
- Opina sobre la legibilidad del barrado personalizado: "¿Se entiende dónde está cada pulso?"

### Puesta en común (7 min)

Preguntas para guiar la discusión:
- "¿Qué fue más difícil: el tresillo o el quintillo? ¿Por qué?" (Esperado: el quintillo, porque 5 notas en un tiempo requieren más control y se nota más si no son uniformes.)
- "Cuando aplicaron puntillos, ¿algún compás les quedó desbalanceado? ¿Cómo se dieron cuenta?" (Contando los tiempos; si no cuadra, hay un puntillo mal puesto o una figura de más/menos.)
- "¿Qué criterio usaron para modificar el barrado? ¿Agruparon por pulso o por frase musical?" (Discutir que ambas opciones son válidas según el contexto: el barrado por pulso ayuda a leer la métrica; el barrado por frase puede reflejar mejor la intención musical.)
- "¿Notaron diferencia auditiva entre la apoyatura y la acciaccatura? ¿Cuál 'roba' más tiempo?"

### Resumen del docente (5 min)

1. Los valores irregulares no son "trampas" rítmicas: son una herramienta de notación para escribir divisiones que no son potencia de 2. El tresillo es el más común, pero el principio es el mismo para cualquier número.
2. **Regla de oro**: primero la duración del grupo completo, después la división. Si invertís el orden, MuseScore te dará un resultado que no esperás.
3. El puntillo es simple matemáticamente (suma la mitad) pero requiere precisión en la escritura. El `.` va ANTES de la nota, como si estuvieras "preparando" la duración extendida.
4. El barrado no es decorativo: comunica la estructura métrica al intérprete. Un barrado mal hecho puede hacer que una pieza fácil parezca difícil de leer.
5. Las notas de adorno son elementos expresivos que MuseScore maneja bien en la reproducción, pero recordá: la apoyatura toma tiempo de la nota principal (la mitad en figuras binarias), la acciaccatura es casi instantánea.

---

## Posibles dificultades

| Problema | Solución |
|---|---|
| El estudiante presiona `Ctrl + 3` antes de seleccionar la duración y obtiene un tresillo "microscópico" | Mostrar el error en tiempo real y luego la forma correcta. Es el error más común. Regla nemotécnica: "primero el espacio, después la división". |
| El tresillo suena "cojo" (las notas no son uniformes) | Posible causa: las notas dentro del tresillo no tienen todas la misma duración. Verificar que cada nota del tresillo tenga el valor correcto. Para un tresillo de corcheas, las tres deben ser corcheas. |
| El quintillo o sextillo "no cierra" el compás | Verificar la duración base: quintillo sobre negra (`5` + `Ctrl + 5`) produce 5 notas en 1 tiempo. Si usaste blanca (`6`), produce 5 notas en 2 tiempos. La duración del grupo debe ser coherente con el compás. |
| El estudiante ingresa el puntillo DESPUÉS de la nota y no funciona | En modo de ingreso, el puntillo debe ir después de la duración y **antes** de la altura. Si la nota ya está escrita, el `.` no la modifica. Para agregar un puntillo a una nota ya escrita, usar el panel de propiedades o salir del modo ingreso. |
| El barrado personalizado "no se nota" en el PDF | Algunos cambios de barrado son sutiles. Sugerir al estudiante que haga cambios drásticos primero (romper TODAS las barras de un compás) para ver el efecto claramente, y luego refinar. |
| La barra sobre el silencio no se aplica | Asegurarse de que el silencio esté entre dos notas que normalmente se agruparían. Seleccionar el silencio y elegir "Unir barras" (no "Romper barra izquierda"). Si aún no funciona, verificar que la nota anterior no tenga "Sin barra" activado. |
| La nota de adorno desplaza rítmicamente las notas siguientes | Las notas de adorno toman su duración de la nota principal que adornan. Si después de la nota con adorno hay un silencio, puede parecer que el ritmo se desplazó cuando en realidad el compás sigue cuadrando. Reproducir el compás completo y verificar que la suma de duraciones sea correcta. |

---

## Recursos adicionales para el docente

- [MuseScore Studio Handbook — Tuplets](https://handbook.musescore.org/notation/rhythm-meter-and-measures/tuplets.md)
- [MuseScore Studio Handbook — Beams](https://handbook.musescore.org/notation/rhythm-meter-and-measures/beams.md)
- [MuseScore 3 Handbook — Tuplets](https://musescore.org/en/handbook/3/tuplets)
- [MuseScore 3 Handbook — Beams](https://musescore.org/en/handbook/3/beams)
- [MuseScore 3 Handbook — Grace notes](https://musescore.org/en/handbook/3/grace-notes)
- **Preparación del archivo de ejercicio** (`ejercicio_S08_ritmo.mscz`): crear partitura para piano (gran pentagrama) en Do mayor, 4/4, 24 compases. Mano derecha con melodía activa (corcheas, semicorcheas) en c.1–12; mano izquierda con acompañamiento simple (blancas, redondas). Compases 13–24 vacíos. Verificar que el ámbito y la dificultad sean accesibles para que el foco esté en el ritmo, no en la lectura de notas.
- Dato curioso: el tresillo es tan común que en algunos estilos (swing, shuffle) se asume implícitamente: las corcheas se interpretan como tresillo corchea-negra aunque estén escritas como corcheas normales. MuseScore tiene una opción de reproducción swing en el panel de reproducción.
- Ejercicio opcional de ampliación para estudiantes avanzados: crear un compás en 4/4 que contenga simultáneamente un tresillo de corcheas en la mano derecha y corcheas normales en la izquierda (polirritmia 3 contra 2). Esto se logra usando voces independientes.

---

*Guía docente — Tecnología Musical I | Sesión 8*
