# programon-equipo

Las herramientas del equipo de Programon. Quien abre esta carpeta es alguien que **lleva
proyectos, no que programa** — PM, cuentas, contenido.

**Tono:** rioplatense, directo, sin emojis. Nada de rutas de archivos, JSON ni jerga técnica en
lo que le mostrás a la persona: no le sirve y la asusta. Si algo falla, decí qué pasó y qué
hacer, no pegues el stack trace.

## Dónde vive cada cosa

Esta es la regla que hace que el sistema sirva, y la que más fácil se rompe.

| Qué | Dónde | Cómo se toca |
|---|---|---|
| Tareas, fases, fechas, responsables, horas | **Tasks** | por el conector de Claude |
| El porqué: decisiones, minutas, cómo habla el cliente | **Tasks**, en las notas del proyecto | `write_project_note` |
| Material del cliente, transcripciones de Meet, entregables | **Google Drive** | por el conector de Drive |
| Skills y convenciones | **Este repo** | solo lo edita Joaquín |

**Nadie escribe archivos acá.** Esta carpeta es de solo lectura para el equipo: es el envase de
las herramientas, no el lugar donde vive el trabajo. Si te dan ganas de crear un `.md` con el
estado de un proyecto, esa es la señal de que va a Tasks.

### La frontera entre una tarea y una nota

- **Si se puede tildar, es una tarea.** Qué falta, quién lo hace, para cuándo.
- **Si explica algo, es una nota.** Por qué se decidió, qué dijo el cliente, cómo se hizo.

Escribir el estado en una nota es el principio de la divergencia: en una semana la nota y las
tareas se contradicen y nadie sabe cuál vale. Es exactamente como Notion se volvió inservible
acá. Si ves una nota que enumera pendientes, convertila en tareas y borrala.

## Antes de trabajar sobre un proyecto

Pedí `get_project_context`. Devuelve en una sola llamada para quién es, cuándo se entrega,
cuánto avanzó, quiénes lo trabajan, los links, los contactos **y las notas**. Te ahorra seis
llamadas y todas las preguntas que el sistema ya sabe responder.

## Lo que no se hace

- **No inventar lo que no está en la fuente.** Si armás una minuta, cada afirmación tiene que
  poder señalarse a una frase literal de la transcripción. Los resúmenes automáticos de
  reuniones fabrican hechos y nombres — ya pasó dos veces y costó caro.
- **No administrar el workspace desde Claude.** Invitar gente, cambiar roles y emitir
  credenciales se hacen desde la pantalla de Tasks, a propósito. Si te lo piden, decí dónde
  está el botón.
- **No instalar skills de terceros.** Si aparece una que parece útil, proponela y que la revise
  Joaquín. Una skill es código que corre con tus permisos.

## Cómo se actualiza esto

Las skills llegan solas: cuando Joaquín publica una versión nueva, Claude la levanta en la
sesión siguiente. Este archivo se actualiza con un `git pull`, que también hace Claude si se lo
pedís.
