---
description: Cuando lo que se habló con el cliente está en WhatsApp — "qué me dijo por WhatsApp", "buscá lo que me mandó Kevin", "pasá a tareas lo que quedó en el grupo", "confirmame si le avisé por WhatsApp". También cuando alguien quiere que Claude lea o escriba en WhatsApp y todavía no está conectado.
---

# WhatsApp

Con varios clientes el canal real es WhatsApp, así que ahí viven decisiones que no están en ningún
otro lado. Se lee con `wacli`, una herramienta de línea de comandos que corre en la computadora de la
persona y habla con su propio WhatsApp.

**Es opcional.** Si la persona no lo quiere conectar, no insistas: el resto de las herramientas
funciona igual.

## Si todavía no está instalado

**Lo instalás vos**, no le pases comandos a nadie. Es un paquete de Homebrew (`openclaw/tap/wacli`)
y el enlace inicial se hace escaneando un QR con el teléfono — eso último es lo único que hace la
persona, porque es su cuenta.

Antes de instalar, decile en una línea qué implica: Claude va a poder leer sus conversaciones de
WhatsApp desde su computadora, y los mensajes quedan en una base local, en su máquina. Si duda, no lo
instales.

## La regla que más se rompe: sincronizar antes de buscar

**El historial local no se actualiza solo.** Si buscás sin sincronizar primero, te va a faltar lo
último — y lo peor es que no falla: contesta con datos viejos como si estuvieran completos.

Así que **antes de cualquier búsqueda, sincronizá**, y recién después buscá. Nunca afirmes que algo
"no está en WhatsApp" sin haber sincronizado en ese mismo momento: ya pasó, y la conclusión fue al
revés de la realidad.

## Cómo se trabaja

1. Sincronizá.
2. Buscá por contacto o por texto. Los nombres de los contactos son como los tiene guardados la
   persona, no el nombre formal del cliente: si no aparece "Interlatina", probá con el nombre de pila.
3. **Leé el hilo completo antes de concluir.** Un mensaje suelto sin lo que vino después dice
   cualquier cosa.
4. Lo que aparezca y sirva —una decisión, un pedido, una fecha— **no se queda en WhatsApp**: la
   decisión va a las notas del proyecto y el pedido a una tarea. Es material que hoy se pierde entero.

## Escribir

**Un mensaje de WhatsApp se muestra antes de mandarse, siempre**, igual que un mail: a quién, y el
texto completo. Es más informal que un mail y por eso más fácil de mandar de más.

Nada de mensajes largos ni de bullets: es un chat. Si lo que hay que decir necesita tres párrafos, es
un mail.

## Lo que no va

- **No leas conversaciones personales.** Si el hilo no es de trabajo, no lo abras y no lo cites.
- No cites textual a un cliente en un lugar donde lo vea otro cliente.
- No asumas que algo se avisó porque estaba en el borrador de un mensaje. Se avisó si se mandó.
