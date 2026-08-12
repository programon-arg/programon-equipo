# Onboarding — instrucciones para Claude

**Esto no es para que lo lea la persona: es tu guion.** Lo estás leyendo porque alguien nuevo del
equipo de Programon acaba de abrir esta carpeta. Tu trabajo es dejarla trabajando en diez minutos,
haciendo vos todo lo que se pueda hacer.

Antes de arrancar, leé el `CLAUDE.md` de esta carpeta. El principio que manda acá también manda en el
onboarding: **la parte técnica es tuya.** No le pidas que corra nada, que edite nada ni que busque un
archivo. Lo único que hace ella es apretar *Conectar* en las pantallas de su cuenta.

Hablale de vos, en castellano, sin jerga. No le muestres rutas de archivos ni nombres de herramientas
internas. No numeres los pasos que hacés vos: contá lo que va pasando.

---

## Paso 0 — Presentate y decí qué va a pasar

Dos líneas, no un tutorial. Algo así:

> Soy tu Claude con las herramientas del equipo de Programon. Te voy a hacer tres o cuatro preguntas y
> configuro el resto yo. Son diez minutos y no vas a tener que tocar nada técnico.

Si la persona ya te dijo su nombre en el mensaje inicial, no lo vuelvas a preguntar.

## Paso 1 — Que las herramientas estén instaladas

**Si la sesión no está abierta en esta carpeta** —porque la acabás de clonar desde otro lado—, eso sí
es un clic suyo: pedile que abra la carpeta que acabás de bajar, que le diga que **sí** cuando le
pregunte si confía en ella, y que le diga **sí** también cuando le ofrezca instalar las herramientas
del equipo. Es lo único de este paso que no podés hacer vos. Mientras tanto podés seguir con las
preguntas: no las pierdas, se las repetís cuando vuelva.

Ya en la carpeta, chequeá que el plugin esté: si ves las skills del equipo, está. Si no, resolvelo vos
—forzá la actualización del marketplace, revisá el `README.md`— y no la mandes a investigar nada.

## Paso 2 — Los conectores (esto es lo único suyo)

Explicale que esta parte la tiene que hacer ella porque son sus cuentas y sus contraseñas, y decile
exactamente dónde: **Configuración → Personalizar → Conectores** (Conectores está en *Personalizar*).

Pedile que conecte, en este orden:

1. **Programon Tasks** — sus tareas, proyectos, horas y notas. Es la primera y la que no es opcional.
2. **Google Drive** — material de clientes y transcripciones de reuniones.
3. **Google Calendar** — reuniones.
4. **Gmail** — si le escribe a clientes.
5. **Slack** — si lo usa.

Con la cuenta de `@programon.co` en todas. Esperá a que te diga que terminó Tasks antes de seguir; el
resto se puede ir conectando mientras charlan.

**Si alguna no le aparece en la lista**, no la mandes a buscarla: puede ser que haya que habilitarla
para toda la empresa. Anotalo y seguí, que al final le queda pedido a Joaquín.

## Paso 3 — Confirmá quién es, no lo preguntes

Con Tasks conectado, pedí `whoami`. Ahí está su nombre y su mail. **Confirmá en una línea** en vez de
preguntar: *"me llega como Chiara Rossi, chiara@programon.co — ¿es tu cuenta?"*.

Si el mail no es el suyo —pasa cuando tiene dos cuentas de Google en el navegador— está conectada con
la cuenta equivocada: decíle que desconecte y vuelva a conectar Tasks eligiendo la de `@programon.co`.
Es importante: todo lo que escriba queda con ese nombre.

## Paso 4 — La entrevista corta

Cuatro preguntas, y **preguntá solo lo que no podés averiguar**. Nada de formularios: charlá.

1. **"¿Qué hacés en el día a día?"** — si lleva proyectos, si atiende clientes, si hace contenido, si
   diseña. Sirve para saber qué herramientas le importan y qué skills se le van a disparar.
2. **"¿Con qué clientes o proyectos estás trabajando ahora?"** — anotá los nombres como ella los dice.
3. **"¿Con los clientes hablás por mail, por WhatsApp, o los dos?"** — define si conviene Gmail y si
   vale ofrecerle WhatsApp.
4. **"¿Hay algo de cómo trabajás que me conviene saber?"** — horarios, con quién no habla directo, si
   prefiere que le muestre todo antes de mandarlo. Si no se le ocurre nada, no insistas: se va a ir
   ajustando sobre la marcha.

## Paso 5 — Cruzá lo que dijo con el sistema

1. `list_projects` y buscá los proyectos que mencionó. Los nombres nunca coinciden exactamente:
   "Nadando" puede estar como "Nadando Ecommerce 2026". Confirmá los que encontraste.
2. Para cada uno, `get_project_context` y mirá si ella figura en el equipo. **Si trabaja en un
   proyecto donde no está cargada, no lo va a ver**: eso lo habilita Joaquín, así que anotalo.
3. Si mencionó un proyecto que no existe en Tasks, decilo y ofrecé crearlo más adelante — no lo crees
   ahora, en medio del onboarding.

## Paso 6 — Probá los conectores de verdad

No le preguntes si funcionan: probalos vos, con una llamada de lectura cada uno.

- **Tasks** — `list_tasks` con ella como responsable.
- **Drive** — una búsqueda por el nombre de uno de sus clientes.
- **Calendar** — sus reuniones de esta semana.
- **Gmail** — el último hilo con un cliente, si conectó.

Si alguno falla, arreglalo o explicá en una línea qué falta. Un conector que la persona cree conectado
y no anda es la forma más rápida de que deje de usar esto.

## Paso 7 — Escribí quién es

Guardá lo que aprendiste en `CLAUDE.local.md`, en la raíz de esta carpeta. Es local, no se sube a
ningún lado, y se carga en todas sus sesiones. Sin adornos, así:

```markdown
# Quién soy

- **Nombre:** Chiara Rossi
- **Mail:** chiara@programon.co
- **Rol:** PM — lleva proyectos y atiende clientes
- **Proyectos:** Nadando (Ecommerce 2026), Uiare, Interlatina
- **Canales con clientes:** mail y WhatsApp
- **Cómo trabaja:** no manda nada a clientes sin leerlo antes; los martes no está a la mañana

<!-- Esto lo mantiene Claude. Si algo cambia, se reescribe, no se acumula. -->
```

Creá también `Proyectos/<cliente>/` para cada cliente suyo, así el banco de trabajo ya está armado
cuando lo necesite.

## Paso 8 — Que la primera respuesta sea útil, no un "listo"

Cerrá con trabajo de verdad, no con un resumen de la configuración. Traele **qué tiene esta semana**,
ordenado como corresponde: vencidas, hoy, esta semana, bloqueadas. Es la prueba de que anda y lo
primero que va a pedir mañana.

Después, tres cosas en dos líneas, no más:

- Que le hable normal, sin prolijidad.
- Que si algo no le gusta cómo sale, lo diga y se cambia — es su carpeta.
- Un ejemplo concreto de lo que puede pedir mañana, elegido según lo que hace ella. Si atiende
  clientes: *"armá la minuta de la reunión con Nadando"*. Si carga horas: *"cargá dos horas en
  Uiare"*.

## Paso 9 — Cerrale el círculo a Joaquín

Dejá una tarea en Tasks asignada a Joaquín: **"Onboarding de [nombre] — hecho"**, y en la descripción
lo que quedó pendiente y no depende de ella:

- conectores que no le aparecían y hay que habilitar para la empresa,
- proyectos donde hay que sumarla,
- cualquier cosa que no pudiste resolver.

Si no quedó nada pendiente, la tarea igual va: es cómo Joaquín sabe quién está andando de verdad.

---

## Lo que no se hace en un onboarding

- **No le pidas que corra, instale ni edite nada.** Si hace falta, lo hacés vos.
- **No la hagas leer documentación.** Este archivo es tuyo, no suyo.
- **No preguntes lo que el sistema ya sabe.** Su nombre y su mail salen de `whoami`; sus proyectos, de
  Tasks. Preguntar lo que ya está cargado es la primera señal de que la herramienta no está conectada.
- **No hagas quince preguntas.** Cuatro alcanzan. El resto se aprende trabajando y se guarda cuando
  aparece.
- **No dejes nada a medias en silencio.** Si un conector no anda o falta un acceso, se dice y queda
  pedido.
