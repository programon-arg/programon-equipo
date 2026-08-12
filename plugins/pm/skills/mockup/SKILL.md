---
description: Cuando hay que mostrar una idea en vez de explicarla — "armá un mockup de la home", "hacé un prototipo de cómo quedaría", "mostrale al cliente cómo se vería", "necesito una pantalla de ejemplo para la reunión", "armá un antes y después". También para una tabla o un gráfico que se va a presentar.
---

# Mostrar una idea

Una pantalla de ejemplo cierra en diez segundos una discusión que por mail lleva tres días. Sirve
para eso: **alinear rápido**, no para entregar diseño.

Se arma como una página publicada —un artifact— que nace **privada** y te deja un link para
compartir. El cliente lo abre en el teléfono, sin instalar nada.

## Antes de arrancar

Una sola pregunta: **¿qué decisión tiene que tomar quien lo mira?** Un mockup que no está hecho para
decidir algo es decoración y genera comentarios de color en vez de una definición.

Traé el contexto del proyecto con `get_project_context`: cómo habla el cliente y qué se decidió ya.
Un prototipo que contradice una decisión anterior reabre lo que estaba cerrado.

## Los criterios

- **El look sale de algún lado real**, no de tu gusto: el sitio del cliente, su marca, o
  `programon.co` si es algo nuestro. Si no hay referencia, decilo y usá algo neutro y sobrio antes
  que inventar una identidad.
- **Una idea por pantalla.** Si hay tres cosas para decidir, son tres pantallas.
- **Texto real, no relleno.** El cliente lee lo que dice. Un titular de mentira se discute como si
  fuera la propuesta de copy.
- **Mirá cómo queda en el teléfono.** Lo va a abrir ahí, no en un monitor.
- **Que se banque el modo oscuro**, o el cliente ve un rectángulo blanco quemado en el celular.

## Los números son la parte peligrosa

**No inventes datos en algo que se le muestra a alguien.** Un dashboard de ejemplo con métricas
inventadas se saca de pantalla y se cita como si fueran nuestros números — y de ahí no se vuelve.

Si hace falta llenar una tabla o un gráfico para que se entienda la forma, que **diga que son datos
de ejemplo**, visible en la pantalla, no en una nota al pie.

## Lo que un mockup no es

- **No es el diseño.** Es una conversación. Cuando la idea está aprobada, el diseño real lo hace
  quien diseña. Decilo cuando lo entregás, así nadie lo toma por definitivo.
- **No es el producto.** Si esto se va a construir, el equipo lo hace en el stack de la casa
  —Next.js con Tailwind, componentes de shadcn sobre Base UI—, así que no prometas nada que dependa
  de cómo quedó armado el prototipo.
- **Nunca uses la marca de otra empresa como si el trabajo fuera de ellos**, ni armes algo que imite
  una comunicación real de un tercero.

## Al terminar

Pasá el link y decí en una línea qué es y qué no: *"es una pantalla de ejemplo para decidir el
orden de las secciones, los textos y los números son de muestra"*. Si de la charla salen
definiciones, dejalas escritas en el proyecto — un mockup aprobado por WhatsApp no es una decisión
registrada.
