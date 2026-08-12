---
description: Cuando arranca un proyecto nuevo o entra un cliente nuevo — "creá el proyecto X", "arrancamos con Y", "dimos de alta a Z", "hay que abrir el proyecto de…". También cuando un proyecto ya existe en el sistema de administración y hay que traerlo.
---

# Arrancar un proyecto

Un proyecto que nace bien cargado se explica solo. Uno que nace con el nombre y nada más
obliga a preguntar lo mismo cinco veces.

## Primero: ¿ya existe del otro lado?

Muchos proyectos ya están en el sistema de administración, con su cliente y sus fechas. **Traer
uno de ahí es mejor que crearlo de cero**: queda vinculado y las horas se imputan al cliente
correcto para la facturación.

Preguntá si el proyecto ya está en el admin antes de crear nada. Si sí, decilo y pedile a
Joaquín o a un admin que lo importe desde **Ajustes → Puente con el admin** — es una pantalla,
lleva diez segundos, y no se puede hacer desde acá.

Si es un proyecto interno o todavía no está del otro lado, seguí.

## Cómo

1. `create_project` con el nombre. El slug sale solo.
2. `write_project_note` de tipo `context` — **este es el paso que la gente saltea y es el que
   importa**. Ver abajo qué va adentro.
3. `add_project_contact` con quién atiende del lado del cliente. Alcanza el nombre; marcá
   `isPrimary` en el que contesta primero.
4. `add_project_link` con lo que ya exista: la carpeta de Drive, el staging, el repo, el
   documento de la propuesta. Si el cliente todavía no tiene carpeta en Drive, armala con la
   convención de dos niveles — ver la skill `drive` — y cargá el link acá.
5. Si ya se sabe cómo se divide, `create_phase` por etapa con sus fechas. Si todavía no, no
   inventes fases: un roadmap de mentira es peor que ninguno.

## La nota de contexto

Es lo que va a leer alguien que caiga en el proyecto dentro de tres meses. Cuatro cosas:

- **Qué es y para quién.** Una línea.
- **Cómo habla el cliente.** Qué palabras usa, qué le importa, qué lo pone nervioso.
- **Cómo se trabaja acá.** Cada cuánto se reporta, quién aprueba, por dónde se habla.
- **Lo que ya se decidió antes de arrancar**, si hubo algo en la venta.

Si no tenés estos datos, **preguntalos ahora**. Es el único momento en que alguien los tiene
frescos; después nadie los va a cargar.

## Al terminar

Decí qué creaste y qué quedó sin cargar, con nombre. *"Falta el contacto del cliente y la
carpeta de Drive"* sirve; *"listo"* deja un proyecto a medias que nadie va a completar.

Y avisá que sumar gente al proyecto se hace desde la pantalla, no desde acá.
