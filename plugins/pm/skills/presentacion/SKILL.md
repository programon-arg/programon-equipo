---
description: Cuando hay que armar lo que se muestra en una reunión con el cliente — "armá la presentación del viernes", "preparame el avance para mostrarle a Uiare", "necesito el reporte de campaña para la reunión", "armá el deck de resultados". También para la reunión semanal de un proyecto de growth.
---

# La presentación de una reunión

Es lo que se muestra mientras alguien habla, no un documento que se manda. Esa diferencia define
todo: **poco texto por pantalla, y una sola idea por pantalla.**

Y a la vez tiene que aguantar que la reabran sin nosotros: el cliente la mira otra vez el lunes, o se
la muestra a su jefe. Así que cada pantalla se tiene que entender sola.

## Dónde vive

**En Drive, en la carpeta del proyecto del cliente, en formato de Google.** Nunca un archivo suelto
en la computadora de alguien: no lo encuentra nadie más y no se puede comentar.

El contenido —qué se dice, en qué orden, los números— va en un **Documento de Google** que se crea
directo en la carpeta del cliente. Ese es el que se trabaja y el que queda. Si además hace falta el
deck para proyectar, se genera y se sube a Drive **convertido a Presentación de Google**; el archivo
intermedio queda en `Proyectos/<cliente>/` y no se le manda a nadie.

Si la reunión es interna o para ordenar una idea, alcanza con el Documento. No armes un deck porque
queda más prolijo.

## La estructura por defecto

Cuatro bloques, en este orden. **El orden importa más que el contenido:** empieza por lo que pasó y
termina en lo que sigue, con el pedido en el medio, que es donde la atención está más alta.

1. **Qué se hizo desde la última vez.** Hechos, no esfuerzo. "Se publicaron 8 piezas y se rearmó el
   catálogo", no "trabajamos mucho en contenido".
2. **Qué muestra eso.** Los números si el proyecto los tiene, con **período y fuente**. Sin período
   un número no dice nada, y sin fuente no se puede discutir.
3. **Qué necesitamos de ellos.** Decisiones pendientes y material que falta, con nombre y para
   cuándo. **Es la pantalla más importante de toda la presentación** y la que más se olvida: la
   mitad de los proyectos que se atrasan lo hacen esperando algo del cliente que nunca se pidió
   así, en claro.
4. **Qué sigue.** Lo próximo con fechas, salido de las tareas del proyecto, no de lo que suena bien.

**Esto es un punto de partida, no un molde fijo.** Cada proyecto y cada equipo lo ajusta —si querés
cambiar las secciones para siempre, pedilo y queda cambiado (ver `ajustar`).

## De dónde salen los datos

- El avance, las fases y lo que sigue: del proyecto en Tasks (`get_project_context`, `list_tasks`).
- Las horas, si el proyecto tiene bolsa contratada: `time_report`, y decí cuánto queda, no cuánto se
  usó.
- Los números de campaña o de tráfico: de donde se miden. **Si no los pudiste ver, no los pongas.**
  Un número inventado en una pantalla que el cliente fotografía es lo peor que puede pasar acá.

## Cómo no suena

- **No maquilles.** Si algo salió mal, va temprano y con qué se está haciendo al respecto. El cliente
  ya lo sabe; enterarse de que nosotros no lo dijimos es peor que el problema.
- **Nada de "estamos trabajando en".** O se hizo, o no se hizo y hay una fecha.
- **Nada de métricas para contemplar.** Porcentajes de avance globales, cantidad de tareas cerradas:
  no llevan a ninguna decisión y ocupan el lugar de lo que sí.
- Sin jerga nuestra. Si el cliente le dice "la web", no le digas "el front".

## Al terminar

Pasá el link del documento en Drive y decí en una línea qué falta para que esté lista —un número que
no pudiste verificar, una decisión que hay que confirmar antes de mostrarla. Y si de la reunión salen
definiciones, esas van a las notas del proyecto: la presentación no es el registro.
