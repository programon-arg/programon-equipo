# programon-equipo

Las herramientas del equipo de Programon para Claude Code.

**Si sos del equipo y llegaste acá: abrí [EMPEZA-ACA.md](EMPEZA-ACA.md).** Son cinco pasos y
no hace falta saber programar.

## Qué hay adentro

- `plugins/pm/` — el plugin con las skills del equipo y el agente `lector`.
- `CLAUDE.md` — cómo trabaja Claude en este contexto: el tono y, sobre todo, **dónde vive cada
  cosa**. Es la regla que hace que el sistema sirva.
- `contexto/` — el vocabulario de la agencia: cómo se llama cada cosa y quién es quién.
- `Proyectos/` — banco de trabajo local de cada persona. No se versiona.

## Las skills

| Skill | Cuándo se dispara |
|---|---|
| `contexto` | "contame cómo viene Interlatina", antes de una reunión de cliente |
| `mi-semana` | "qué tengo hoy", "por dónde arranco" |
| `avanzar` | "terminé el wireframe", "estoy trabada esperando al cliente" |
| `horas` | "cargá dos horas en Interlatina", "cuánto lleva el proyecto" |
| `delegar` | "pasale esto a Franco", "que lo siga Consuelo" |
| `decision` | "anotá que decidimos…", cuando algo se va a perder si nadie lo escribe |
| `minuta` | "armá la minuta de la reunión con Honda" |
| `mail` | "armá el mail para Inés", "contestale al cliente" |
| `drive` | "dónde está el logo de Uiare", antes de crear una carpeta de cliente |
| `arrancar-proyecto` | "creá el proyecto X", "arrancamos con Y" |
| `estado-semanal` | "el resumen para la reunión del lunes" |
| `buscar-skill` | cuando algo se hace a mano y repetido |

Y un agente: `lector`, read-only, para digerir transcripciones y hilos largos sin ensuciar el
contexto principal.

## Cómo se actualiza

`plugin.json` **no declara versión a propósito**: la versión se resuelve del commit, así que
mergear a `main` alcanza para que a cada persona le lleguen los cambios en la sesión siguiente. Si
declarás un `version`, el plugin queda pineado en ese string y nadie recibe nada hasta que lo
bumpees. El resto del repo se actualiza con `git pull`.

Para forzarlo en el momento: `/plugin marketplace update programon`.

**Nadie del equipo escribe acá** —salvo en su `Proyectos/` local. Las tareas, las notas y las
decisiones viven en [Tasks](https://tasks.programon.co); el material del cliente, en Drive.
