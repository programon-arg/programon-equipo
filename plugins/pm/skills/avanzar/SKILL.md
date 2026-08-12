---
description: Cuando alguien cuenta que algo avanzó, se terminó o se trabó — "terminé el wireframe", "ya mandé la propuesta", "esto quedó listo", "pasá a revisión la home", "estoy trabada esperando al cliente", "marcá como hecho lo de Honda". También cuando hay que dejar dicho en una tarea qué pasó.
---

# Mover una tarea

Es lo que más veces al día se hace y lo que más se saltea, porque abrir la pantalla para tildar
una casilla no vale el viaje. Acá vale: se dice y queda.

## Cómo

1. **Encontrá la tarea.** `search_tasks` con las palabras que usó la persona. Si sabés el proyecto,
   `list_tasks` filtrando por ese proyecto sale más limpio.
2. **Si hay más de una que puede ser, preguntá cuál.** Mover la tarea equivocada es peor que no
   mover ninguna: la de al lado queda mintiendo.
3. `update_task` con el estado nuevo. Los cuatro son `pending`, `in_progress`, `blocked` y
   `completed`.
4. **Si contó *por qué*, `add_comment`.** El estado dice dónde está; el comentario dice qué pasó, y
   es lo que lee el resto del equipo. "Trabada" sin motivo obliga a preguntar por Slack.

## Cuando se trabó

`blocked` no es "me está costando": es **depende de otro**. Preguntá de quién o de qué depende y
ponelo en el comentario con nombre. Un bloqueo sin dueño no se destraba nunca.

Si lo que falta es que alguien haga algo concreto, eso es una tarea aparte de esa persona — ofrecé
crearla con `create_task` en vez de dejarla escrita solo en el comentario.

## Cuando se terminó

Antes de dar por cerrada una tarea, mirá si quedó algo colgando de lo que contó: "terminé el
wireframe y se lo mandé al cliente" cierra una tarea y **abre** la de esperar la devolución. Ofrecé
crearla, no la crees sola.

## Al terminar

Decí en una línea qué cambiaste, con el título de la tarea. Si de paso cargaste horas o creaste
otra tarea, decilo también. Nada de "listo".

## Lo que no va

- No cambies fechas de entrega para que deje de estar vencida. Una tarea vencida es información.
- No cierres varias de una porque "seguro también están hechas". Solo lo que la persona dijo.
