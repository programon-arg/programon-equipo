---
description: Cuando alguien pregunta cómo viene un proyecto, pide ponerse al día con uno, va a una reunión de cliente, o dice "contame de X", "en qué está Y", "necesito el estado de Z". También antes de trabajar sobre un proyecto que no conocés.
---

# El estado de un proyecto

Una sola llamada trae todo. **Empezá siempre por ahí**, incluso si creés que ya sabés el
estado: el proyecto cambió desde la última vez.

## Cómo

1. `list_projects` si no tenés el id — la persona te va a decir "Interlatina", no un uuid.
2. `get_project_context` con ese id. Devuelve cliente, fechas, avance, fase actual, equipo,
   links, contactos **y las notas**, que son el porqué del proyecto.
3. Si hace falta el detalle de qué está pendiente, `list_tasks` filtrando por el proyecto.

No llames a `list_phases`, `list_members` ni `add_project_link` para completar: ya vino todo en
el paso 2.

## Qué contestar

Escribí para alguien que va a entrar a una reunión en cinco minutos. En este orden:

1. **Una línea de qué es y para quién.** Sale de las notas de tipo contexto.
2. **Cómo viene:** avance, fase actual, y la fecha de entrega con cuántos días faltan. Si la
   entrega es derivada del roadmap y no comprometida, decilo — se decide distinto con una que
   con la otra.
3. **Lo que está trabado o vencido**, con nombre y responsable. Esto va arriba de lo que está
   bien: nadie necesita que le confirmen que todo marcha.
4. **Las decisiones que explican el estado actual**, de las notas. No todas: las que hacen
   falta para no volver a discutir algo ya resuelto.
5. **A quién se le pregunta**, del contacto principal.

Si algo no está cargado, decí que no está cargado. No lo infieras de las tareas ni lo
completes con lo que parece razonable — un dato inventado en un brief es peor que un hueco,
porque el hueco se nota.

## Cuando no hay nada

Un proyecto sin notas es un proyecto cuyo porqué está en la cabeza de alguien. Decilo y ofrecé
escribirlo: *"no hay ninguna nota de contexto cargada; si me contás en dos líneas de qué se
trata, la dejo escrita para el resto"*.
