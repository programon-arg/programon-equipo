---
description: Cuando alguien quiere dejar algo escrito en un proyecto — "anotá que decidimos X", "guardá esto", "que quede registrado", "el cliente dijo que…" — o cuando en una conversación aparece una decisión que se va a perder si nadie la escribe.
---

# Dejar escrito el porqué

Lo más caro de perder de un proyecto no son las tareas: es **por qué se decidió lo que se
decidió**. Seis meses después alguien vuelve a proponer lo mismo que ya se descartó, y nadie
se acuerda del motivo.

## Antes de escribir, decidí si es una nota

**Si se puede tildar, es una tarea, no una nota.** "Mandar la propuesta el jueves" es una
tarea. "Vamos con Vercel porque el deploy por push es lo que hace que no se posterguen" es una
nota.

Si lo que te dictaron mezcla las dos cosas —pasa siempre—, separalas: la decisión va a la nota
y lo que hay que hacer va a `create_task`. Decí que hiciste las dos cosas.

## Cómo

1. `get_project_context` primero. **Siempre.** No es burocracia: si ya hay una nota de ese
   tema, se edita con `update_project_note` en vez de dejar la quinta versión de lo mismo, que
   es exactamente como esto se vuelve inútil.
2. Elegí el tipo: `decision` para algo que se resolvió, `context` para qué es el proyecto y
   cómo se trabaja, `meeting` para una reunión, `note` para el resto.
3. `write_project_note` con un título que se entienda solo en una lista de veinte.

Cuidado con editar: el `body` **reemplaza** al anterior. Para sumar algo, mandá el texto
completo con lo nuevo adentro, no solo el párrafo nuevo.

## Cómo escribir el cuerpo

Markdown, corto, y **con el motivo adentro**. Una decisión sin su porqué no sirve para nada:
dentro de seis meses lo que hace falta saber no es qué se eligió, es qué se descartó y por qué.

Escribí lo que se dijo, no lo que suena bien. Si la razón real fue "el cliente no quiere pagar
la integración", eso es lo que va — maquillarlo hace que la próxima persona no entienda la
decisión.

Si te dictaron algo ambiguo, preguntá **antes** de escribir. Una nota mal escrita es peor que
ninguna, porque después se cita.
