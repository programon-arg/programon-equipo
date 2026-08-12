# programon-equipo

Las herramientas del equipo de Programon para Claude Code.

**Si sos del equipo y llegaste acá: abrí [EMPEZA-ACA.md](EMPEZA-ACA.md).** Son cuatro pasos y no hace
falta saber programar.

## Los dos principios

**La parte técnica no es de la persona.** Claude no le pide a nadie que corra un comando, edite un
archivo o instale algo: lo hace él. Lo único que hace la persona es apretar *Conectar* en la pantalla
de Google, escanear un QR y aprobar lo que sale para afuera.

**Esto es un blueprint, no un envase cerrado.** Cada uno se lo adapta: el tono, los pasos de una
skill, lo que lleva una presentación. Los cambios son locales, sin push ni pull request. Cuando una
mejora sirve para todos, se sube al plugin y le llega al resto.

## Qué hay adentro

- `plugins/pm/` — el plugin con las skills del equipo y el agente `lector`. **Esto se actualiza solo:
  no editar acá.** Las adaptaciones de cada persona van a `.claude/skills/`.
- `CLAUDE.md` — cómo trabaja Claude en este contexto: los principios, el tono y **dónde vive cada
  cosa**.
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
| `agendar` | "buscá un hueco con el cliente", "preparame la reunión de las 3" |
| `presentacion` | "armá la presentación del viernes", el avance que se muestra en reunión |
| `mail` | "armá el mail para Inés", "contestale al cliente" |
| `whatsapp` | "qué me dijo por WhatsApp" (opcional, hay que conectarlo) |
| `drive` | "dónde está el logo de Uiare", crear un documento del cliente |
| `mockup` | "mostrale al cliente cómo quedaría", "armá una pantalla de ejemplo" |
| `arrancar-proyecto` | "creá el proyecto X", "arrancamos con Y" |
| `estado-semanal` | "el resumen para la reunión del lunes" |
| `ajustar` | "no me gusta cómo hace esto", "quiero que siempre…" |
| `como-anda-claude` | "¿Claude puede hacer X?", "por qué se olvidó de lo que le dije" |
| `buscar-skill` | cuando algo se hace a mano y repetido |

Y un agente: `lector`, read-only, para digerir transcripciones y hilos largos sin ensuciar el
contexto principal.

## Cómo se actualiza

`plugin.json` **no declara versión a propósito**: la versión se resuelve del commit, así que
mergear a `main` alcanza para que a cada persona le lleguen los cambios en la sesión siguiente. Si
declarás un `version`, el plugin queda pineado en ese string y nadie recibe nada hasta que lo
bumpees.

Para forzarlo en el momento: `/plugin marketplace update programon`.

Las adaptaciones locales de cada persona viven en `.claude/skills/` y en su `CLAUDE.md`, así que una
actualización del plugin no las pisa.
