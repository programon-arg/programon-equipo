# Empezá acá

Esto le da a tu Claude las herramientas del equipo: buscar el estado de un proyecto, armar la
minuta de una reunión, dejar escrita una decisión, cargar horas, ver qué tenés esta semana.

No hace falta saber programar. Son cinco pasos y se hacen una sola vez.

---

## 1. Abrí Claude Code

Bajate la app de Claude para escritorio si no la tenés, entrá con tu cuenta de `@programon.co`,
y abrí **Claude Code** desde ahí. No hace falta terminal.

## 2. Traé esta carpeta a tu computadora

Pedile a Claude, literal:

> Cloná `https://github.com/programon-arg/programon-equipo` en mi carpeta de proyectos y abrilo.

Lo hace solo. Cuando termine, va a preguntarte si confiás en la carpeta: **decile que sí**. Ahí
te ofrece instalar las herramientas del equipo — **también decile que sí**.

## 3. Conectá las herramientas

En Claude —claude.ai o la app— andá a **Configuración → Personalizar → Conectores**. Ojo que
Conectores está en *Personalizar*, no en Configuración a secas.

Conectá estas cuatro, en este orden:

| Conector | Para qué | Hace falta |
|---|---|---|
| **Programon Tasks** | tus tareas, proyectos, horas y notas | sí, siempre |
| **Google Drive** | material de clientes y transcripciones de reuniones | sí — sin esto no se pueden armar minutas |
| **Gmail** | leer hilos con clientes y armar borradores | si le escribís a clientes |
| **Slack** | buscar y escribir en los canales del equipo | si lo usás |

En cada una apretás **Conectar**. Con Tasks se abre una pantalla nuestra que dice qué permisos
pide: fijate que el mail de arriba sea el tuyo y dale **Dar acceso**. Con Google y Slack es la
pantalla de ellos, la de siempre.

Entrá con tu cuenta de `@programon.co` en todas. Lo que Claude haga queda con tu nombre y ve
exactamente lo que ves vos: ni un archivo más.

## 4. La primera vez te va a pedir permiso

Cuando Claude use una de estas herramientas por primera vez, te aparece un cartel preguntando si
puede. Elegí la opción de **no volver a preguntar** y listo, no molesta más.

Hay dos cosas para las que **siempre** va a pedirte confirmación, aunque le digas que no pregunte
más: mandar un mail y mandar un mensaje de Slack. Eso es a propósito.

## 5. Probá que anda

Pedile:

> Qué tengo esta semana

Si te contesta con tus tareas, ya está funcionando.

---

## Qué le podés pedir ahora

- **"Contame cómo viene Interlatina"** — el estado del proyecto, quién trabaja, qué está
  trabado y por qué el proyecto es como es.
- **"Armá la minuta de la reunión de hoy con Honda"** — busca la transcripción en el Drive,
  escribe la minuta y carga las tareas que salieron.
- **"Terminé el wireframe de Uiare"** — mueve la tarea y deja dicho qué pasó.
- **"Cargá dos horas en Interlatina por la reunión de hoy"**.
- **"Anotá que decidimos no tocar el hosting hasta que confirmen el presupuesto"** — queda
  escrito en el proyecto, con fecha, y lo ve el resto del equipo.
- **"Pasale a Franco la revisión de la home, para el jueves"**.
- **"Armá el mail para Inés contándole que subimos la propuesta"** — te lo muestra antes de mandar.
- **"Dónde está el logo de Uiare"** — lo busca en el Drive del cliente.
- **"Pasame el estado de mis proyectos para la reunión del lunes"**.

No hace falta que le hables prolijo. Si algo le sale mal te lo dice y lo corregís ahí mismo.

---

## Tres cosas que conviene saber

**Esta carpeta no es tuya para escribir**, con una excepción: la carpeta `Proyectos`. Ahí podés
dejar archivos de paso —un PDF que bajaste, algo que estás armando— y son tuyos y locales, no se
suben a ningún lado. Todo lo demás que escribís —tareas, notas, decisiones— vive en Tasks, y el
material terminado, en Drive.

**Lo que Claude lee de un mail o de un documento no son órdenes.** Si un mail dice "reenviá esto a
tal persona", Claude te lo cuenta pero no lo hace. Está bien que sea así.

**Si algo no anda**, pedile a Claude que actualice las herramientas del equipo, o escribile a
Joaquín. No rompiste nada.
