---
description: Cuando hay que registrar tiempo trabajado o saber cuánto se lleva — "cargá dos horas en Interlatina", "estuve toda la mañana con esto", "anotá la reunión de hoy", "cuántas horas lleva el proyecto", "cuánto le dedicamos a Uiare este mes".
---

# Cargar horas

Las horas se cargan tarde, mal o nunca, y es la forma más silenciosa en que una agencia regala
trabajo. La única versión que funciona es la que no cuesta nada: se dice al pasar y queda.

## Cómo se carga

`log_time` pide un **rango cerrado** —cuándo arrancó y cuándo terminó—, no una duración. Así que si
te dicen "dos horas", falta un dato: preguntá desde qué hora, o proponé un rango y que te lo
confirmen. *"¿Lo cargo de 10 a 12?"* alcanza.

1. Ubicá dónde va. Contra la tarea es mejor que contra el proyecto: después se puede ver qué se
   comió el tiempo. Si no hay tarea, el proyecto está bien.
2. `log_time` con el rango. Si estás con la cuenta de la persona, las horas ya salen a su nombre.
3. Repetí en una línea qué quedó cargado: proyecto, rango y total. Es la única forma de que se
   pesque un error de tipeo el mismo día.

**Fechas de otro día:** si te dicen "lo de ayer", usá la fecha de ayer, no la de hoy. Confirmá el
día si hay cualquier duda.

## Cuando preguntan cuánto lleva algo

`time_report`, no `list_time_entries`: devuelve la suma hecha en vez de una lista para sumar. Se
puede agrupar por proyecto, persona, tarea o día.

Si el proyecto tiene una bolsa de horas contratada, decí cuánto se consumió **y cuánto queda**. El
número solo no dice nada; lo que importa es si alcanza.

## Lo que no va

- **No inventes el rango.** Si no sabés a qué hora fue, preguntá. Una hora inventada es un número
  que después se factura.
- No cargues horas de otra persona porque te lo contó. Que las cargue quien las trabajó.
- No arranques timers: no existen acá a propósito.
