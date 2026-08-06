# Sesión 3: Navegación, selección y reproducción

📚 Handbook → Basics — Viewing and navigation, Selection modes, Undo and redo; Sound and Playback — Play mode | Herramientas: MuseScore Studio 4, Google Classroom

---

??? info "Glosario de términos"
    Consultá esta tabla cuando encuentres un término que no conozcas.

    | Término | Definición |
    |---|---|
    | <a id="zoom"></a> **Zoom** | Ampliación o reducción de la vista de la partitura en pantalla. No modifica el tamaño real de impresión. Se controla con `Ctrl + rueda del ratón` o `Cmd + rueda` en macOS. |
    | <a id="desplazamiento"></a> **Desplazamiento** | Movimiento horizontal o vertical dentro de la partitura para ver secciones que no caben en pantalla. Se hace con las barras de desplazamiento, la rueda del ratón o atajos de teclado. |
    | <a id="vista-pagina"></a> **Vista de página** | Modo de visualización que muestra la partitura como se verá impresa: con saltos de página, márgenes y encabezados. Ideal para revisar el formato final. |
    | <a id="vista-continua"></a> **Vista continua** | Modo de visualización sin saltos de página. Los compases se muestran uno tras otro horizontalmente. Ideal para la etapa de ingreso y edición de notas. |
    | <a id="seleccion"></a> **Selección** | Acción de marcar uno o más elementos de la partitura para editarlos, copiarlos o eliminarlos. Puede ser de un solo elemento, un rango de compases o una región completa. |
    | <a id="deshacer"></a> **Deshacer** | Comando que revierte la última acción realizada. Atajo universal: `Ctrl + Z` (Windows/Linux) o `Cmd + Z` (macOS). MuseScore conserva un historial ilimitado de cambios durante la sesión. |
    | <a id="rehacer"></a> **Rehacer** | Comando que restaura una acción que fue deshecha. Atajo: `Ctrl + Shift + Z` o `Cmd + Shift + Z`. |
    | <a id="reproduccion"></a> **Reproducción** | Ejecución sonora de la partitura usando la biblioteca de sonidos integrada. Se controla desde la barra de transporte o con la tecla `Espacio`. |
    | <a id="metronomo"></a> **Metrónomo** | Señal sonora que marca el pulso durante la reproducción. Se activa y desactiva desde la barra de reproducción. Útil para verificar que el ritmo escrito coincide con la métrica. |
    | <a id="bucle"></a> **Bucle de reproducción** | Repetición continua de un fragmento seleccionado. Se activa con el botón de bucle en la barra de reproducción. Permite escuchar un pasaje repetidamente para detectar errores. |

???+ note "Modos de visualización y control de la vista"

    MuseScore ofrece dos modos principales para visualizar la partitura, cada uno con un propósito distinto en el flujo de trabajo:

    | Modo | ¿Cómo se ve? | ¿Cuándo usarlo? |
    |---|---|---|
    | **[Vista de página](#vista-pagina)** | Páginas individuales con márgenes, saltos y encabezados. Igual a como se imprimirá. | Revisar formato, verificar paginación, preparar la entrega final. |
    | **[Vista continua](#vista-continua)** | Los compases fluyen horizontalmente sin interrupción de páginas. | Ingresar notas, editar, trabajar en pasajes largos sin distracciones de formato. |

    El cambio entre modos se hace desde la barra de herramientas o desde el menú **Ver → Vista de página / Vista continua**.


    ### Zoom y desplazamiento

    El [zoom](#zoom) se controla de varias maneras:

    | Acción | Atajo / Método |
    |---|---|
    | Acercar | `Ctrl + +` (`Cmd + +` en macOS) o `Ctrl + rueda arriba` |
    | Alejar | `Ctrl + -` (`Cmd + -` en macOS) o `Ctrl + rueda abajo` |
    | Ajustar a ancho de página | `Ctrl + 0` (atajo frecuente; varía según versión y sistema) |
    | Desplazar horizontalmente | `Shift + rueda del ratón` o arrastrar la barra inferior |
    | Desplazar verticalmente | `Rueda del ratón` o arrastrar la barra lateral |

    !!! tip "El zoom que ves no es el tamaño de impresión"
        El zoom solo afecta a lo que ves en pantalla. Para cambiar el tamaño real de la partitura impresa, se modifica la escala en **Formato → Estilo → Página**.

    ### Búsqueda de compases

    Para ir rápidamente a un compás específico, usá **Editar → Ir a compás** o el atajo `Ctrl + G` (`Cmd + G`). Ingresá el número de compás y MuseScore te llevará directamente a ese punto.

???+ note "Técnicas de selección"

    En MuseScore, seleccionar correctamente es la base de casi todas las operaciones de edición: copiar, pegar, eliminar, modificar, transponer. Una selección incorrecta produce resultados inesperados.

    ### Tipos de selección

    | Tipo | Cómo se hace | Qué selecciona |
    |---|---|---|
    | **Un elemento** | Clic sobre el elemento | Una nota, un silencio, un texto, una dinámica... |
    | **Rango de compases** | Clic en el primer compás, `Shift + clic` en el último | Todos los compases entre ambos inclusive, con todas sus notas y símbolos |
    | **Compás completo** | Clic en un espacio vacío del compás (no sobre una nota) | Todas las voces y elementos del compás |
    | **Región rectangular** | `Shift + arrastrar` desde un punto a otro | Elementos dentro de un rectángulo visual |
    | **Seleccionar todo** | `Ctrl + A` / `Cmd + A` | Toda la partitura |
    | **Voz específica** | Usar los botones de voz (1, 2, 3, 4) en la barra de herramientas | Solo las notas de la voz seleccionada, ignorando las otras |


    !!! warning "Clic en el lugar correcto"
        Si hacés clic sobre una nota, seleccionás **esa nota**. Si hacés clic en el espacio vacío de un compás, seleccionás **todo el compás**. Si hacés clic sobre un pentagrama pero fuera de los compases, no seleccionás nada. La diferencia es sutil pero fundamental.

    ### Selección con el teclado

    | Atajo | Acción |
    |---|---|
    | `←` / `→` | Mover la selección a la nota o silencio anterior / siguiente |
    | `Ctrl + ←` / `Ctrl + →` | Mover la selección al inicio del compás anterior / siguiente |
    | `Shift + ←` / `Shift + →` | Extender la selección nota por nota |
    | `Shift + Ctrl + ←` / `Shift + Ctrl + →` | Extender la selección compás por compás |

???+ note "Deshacer, rehacer y guardar: la red de seguridad"

    ### Deshacer y rehacer

    MuseScore registra cada acción que realizás durante una sesión de trabajo. El historial de [deshacer](#deshacer) es **ilimitado mientras el archivo está abierto**: podés volver atrás hasta el momento en que abriste la partitura.

    | Acción | Atajo Windows/Linux | Atajo macOS |
    |---|---|---|
    | Deshacer | `Ctrl + Z` | `Cmd + Z` |
    | Rehacer | `Ctrl + Shift + Z` | `Cmd + Shift + Z` |

    También se accede desde **Editar → Deshacer** y **Editar → Rehacer**.

    !!! info "¿Qué pasa al cerrar el archivo?"
        Al cerrar y volver a abrir una partitura, el historial de deshacer se reinicia. Por eso es importante **guardar versiones sucesivas** con números de versión (`_v01`, `_v02`, `_v03`), especialmente antes de hacer cambios estructurales grandes.

    ### Guardar y guardar como

    | Comando | Atajo | ¿Qué hace? |
    |---|---|---|
    | **Guardar** | `Ctrl + S` / `Cmd + S` | Sobrescribe el archivo actual con los cambios recientes. |
    | **Guardar como** | `Ctrl + Shift + S` / `Cmd + Shift + S` | Crea un archivo nuevo con los cambios, conservando el anterior. Ideal para versiones. |

    !!! tip "Estrategia de versiones"
        Antes de una edición grande (transponer, cambiar instrumentos, reorganizar compases), hacé **Guardar como** con el siguiente número de versión. Si algo sale mal, cerrás la versión nueva y volvés a abrir la anterior. Es más seguro que depender solo del historial de deshacer.

???+ note "Reproducción y controles de transporte"

    La reproducción en MuseScore no es solo para "escuchar cómo suena": es una **herramienta de revisión**. Te permite detectar errores de altura, ritmo, armonía y estructura que el ojo puede pasar por alto.

    ### Controles básicos

    | Acción | Atajo / Control |
    |---|---|
    | Reproducir / Pausar | `Espacio` o botón ▶ de la barra de transporte |
    | Reproducir desde el inicio | `Inicio` (tecla) o botón ⏮ |
    | Detener | `Esc` o botón ⏹ |
    | Ir al inicio de la partitura | `Inicio` |
    | Ir al final de la partitura | `Fin` |


    ### Reproducción desde un punto específico

    Hacé clic sobre la nota o compás desde donde querés empezar y presioná `Espacio`. MuseScore reproducirá desde ese punto hasta el final, a menos que lo detengas.

    ### Metrónomo y bucle

    - **Metrónomo**: activalo con el botón del metrónomo en la barra de reproducción. La claqueta sonora te ayudará a verificar que tus ritmos encajan en la métrica del compás.
    - **Bucle**: seleccioná un rango de compases, activá el botón de bucle (⟳) y presioná `Espacio`. El fragmento se repetirá continuamente. Reducí la velocidad con el control de tempo para escuchar pasajes difíciles con más detalle.

    !!! warning "La reproducción no reemplaza la lectura"
        MuseScore reproduce lo que escribiste, no lo que "quisiste escribir". Si ingresaste una nota equivocada, la reproducción la tocará equivocada. La escucha debe complementar la lectura visual, no sustituirla.

---

## Actividad en Classroom

### Tarea: S03 — Ingreso de ritmo con mouse y teclado

Abrí la partitura de referencia disponible en [Google Drive](https://drive.google.com/file/d/18MJa1_UqFADSpKYLNuMhWd0MFYnHkBj_/view).

1. **Creá una partitura nueva** con la misma instrumentación, armadura, compás y tempo que la partitura de referencia.
2. **Ingresá solo el ritmo** de los primeros 2 sistemas usando el **mouse**: colocá las figuras y silencios sin preocuparte por las alturas (usá una misma nota repetida, por ejemplo Do central).
3. **Repetí el mismo ejercicio** usando solo el **teclado** del computador: ingresá el ritmo de esos mismos 2 sistemas sin tocar el mouse.
4. Compará ambas experiencias y anotá en cuál fuiste más rápido y en cuál cometiste menos errores.

### Entregables

- [ ] `APELLIDO_Nombre_S03_ritmo_mouse_v01.mscz`
- [ ] `APELLIDO_Nombre_S03_ritmo_teclado_v01.mscz`
- [ ] Breve reflexión (3–5 líneas) comparando ambos métodos de ingreso

---

*Basado en: MuseScore 3 Handbook — Basics: Viewing and navigation, Selection modes, Undo and redo; Sound and Playback — Play mode | https://musescore.org/en/handbook/3*
