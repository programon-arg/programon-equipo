---
description: Cuando la persona quiere que Claude trabaje distinto — "no me gusta cómo hace X", "quiero que siempre me pregunte antes", "cambiá el formato del resumen", "agregale al informe tal cosa", "esto lo hace mal", "necesito que aprenda a hacer Y", "acordate de que en este cliente…". También cuando corrige lo mismo dos veces.
---

# Cambiar cómo trabajan las herramientas

Estas herramientas son un punto de partida, no una regla. **Si a la persona le molesta cómo sale
algo, se cambia** — en el momento, sin pedir permiso a nadie y sin que ella toque nada.

## La señal de que hay que usar esta skill

**Te corrigió lo mismo dos veces.** Ahí no hay que volver a corregirlo: hay que cambiar la
herramienta para que salga bien la próxima vez. Si no, la persona se convierte en el corrector de
algo que debería aprender.

## Cómo

1. **Entendé qué molesta, no qué pidió.** "Ponelo más corto" puede ser el largo, o puede ser que
   sobra una sección entera. Preguntá una sola cosa si hace falta: *"¿te sobra el detalle de las
   tareas o el orden?"*.
2. **Escribí el cambio donde corresponde:**
   - Cambia cómo sale **una** cosa —una minuta, un resumen semanal, un mail—: la skill de eso.
   - Cambia el **tono o una regla general**: el `CLAUDE.md` de esta carpeta.
   - Es un dato de **un cliente puntual** —cómo se llama, quién aprueba, qué no le gusta—: eso no es
     una skill, va a las notas de ese proyecto en Tasks, donde lo ve el resto del equipo.
3. **La adaptación va a `.claude/skills/<nombre>/SKILL.md` de esta carpeta**, no a `plugins/`. Lo de
   `plugins/` se actualiza solo y una edición ahí choca con la próxima actualización. Si la skill
   viene del plugin, copiala primero y editá la copia.
4. **Contale qué cambiaste en una frase**, sin rutas ni nombres de archivo: *"listo, de ahora en más
   el resumen semanal no lleva porcentajes"*.
5. **Si el cambio le sirve a todo el equipo, dejale la tarea a Joaquín** con el texto del cambio, así
   lo suma a las herramientas de todos. No hace falta que nadie copie nada a mano.

## Qué se puede cambiar

Todo. El tono, los pasos, qué lleva un informe, qué no se hace, agregar una herramienta que no está,
sacar una que molesta. Si la persona pide algo que hoy no existe, **se escribe** — ver `buscar-skill`
para cuándo conviene traer algo de afuera y cuándo escribirlo nosotros.

Lo único que no se cambia por gusto es dónde vive la información: las tareas en Tasks, los
documentos en Drive. Eso no es una preferencia, es lo que evita que en dos semanas haya dos
versiones de la verdad. Si igual lo pide, explicá por qué está así una vez, y si insiste, es su
carpeta: se hace y se le avisa a Joaquín.

## Lo que no va

- **No le pidas que edite nada.** Ni un archivo, ni una línea, ni "cambiá esto acá". Lo hacés vos.
- No pidas confirmación para un cambio reversible en su propia carpeta. Se hace y se cuenta.
- No acumules tres versiones de la misma skill "por si acaso". Se reescribe la que hay.
