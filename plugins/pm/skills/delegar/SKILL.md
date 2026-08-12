---
description: Cuando hay que pasarle trabajo a otra persona — "pasale esto a Franco", "que lo siga Consuelo", "asignale la home a Brian", "delegá el diseño", "esto no es mío, es de Juan". También cuando una tarea sin responsable aparece en un reporte.
---

# Pasarle una tarea a otro

Una tarea sin responsable no la hace nadie, y una asignada sin avisar tampoco. Las dos mitades van
juntas.

## Cómo

1. `list_members` para el id de la persona. La gente te va a decir "Franco", no un uuid; si hay dos
   Francos, preguntá cuál.
2. `assign_task` con la tarea y la persona.
3. **Fecha.** Si no tiene, preguntá para cuándo y ponela con `update_task`. Delegar sin fecha es
   mandar algo al fondo de la lista de otro.
4. `add_comment` con lo que la persona necesita para arrancar: qué se espera, dónde está el
   material, con quién habla. La notificación le llega al nuevo responsable.

El paso 4 es el que hace la diferencia. Asignar sin contexto obliga a la otra persona a reconstruir
la conversación que vos ya tuviste.

## Si la tarea todavía no existe

Créala con `create_task` ya asignada, en el proyecto que corresponda, y aclará que la creaste.

## Lo que no va

- **Sumar gente al proyecto no se hace desde acá**, se hace desde la pantalla de Tasks. Si la
  persona no aparece en `list_members` del proyecto, decí eso y dónde está el botón.
- No reasignes lo que ya está en curso de otro sin decirlo: primero avisá que la tarea tiene
  responsable y desde cuándo.
