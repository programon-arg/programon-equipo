# programon-equipo

Las herramientas del equipo de Programon para Claude Code.

**Si sos del equipo y llegaste acá: abrí [EMPEZA-ACA.md](EMPEZA-ACA.md).** Son cuatro pasos y
no hace falta saber programar.

## Qué hay adentro

- `plugins/pm/` — el plugin con las skills del equipo.
- `CLAUDE.md` — cómo trabaja Claude en este contexto: el tono y, sobre todo, **dónde vive cada
  cosa**. Es la regla que hace que el sistema sirva.
- `pendientes/` — skills propuestas y todavía sin revisar.

## Las skills

| Skill | Cuándo se dispara |
|---|---|
| `contexto` | "contame cómo viene Interlatina", antes de una reunión de cliente |
| `mi-semana` | "qué tengo hoy", "por dónde arranco" |
| `decision` | "anotá que decidimos…", cuando algo se va a perder si nadie lo escribe |
| `minuta` | "armá la minuta de la reunión con Honda" |
| `arrancar-proyecto` | "creá el proyecto X", "arrancamos con Y" |
| `estado-semanal` | "el resumen para la reunión del lunes" |
| `buscar-skill` | cuando algo se hace a mano y repetido |

## Cómo se actualiza

Las skills llegan solas: al bumpear la versión en `plugins/pm/.claude-plugin/plugin.json` y
mergear, Claude las levanta en la sesión siguiente de cada persona. El resto del repo se
actualiza con `git pull`.

**Nadie del equipo escribe acá.** Las tareas, las notas y las decisiones viven en
[Tasks](https://tasks.programon.co); el material del cliente, en Drive.
