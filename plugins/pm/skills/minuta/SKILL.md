---
description: Cuando hay que armar la minuta de una reunión, resumir lo que se habló con un cliente, o sacar las tareas que salieron de un Meet. Trigger con "armá la minuta", "qué salió de la reunión con X", "pasá a tareas lo que hablamos".
---

# La minuta de una reunión

Google Meet guarda la transcripción en el Drive del organizador, como documento, en una carpeta
por reunión. De ahí sale todo.

## La regla que ordena esta skill

**Cada afirmación de la minuta tiene que poder señalarse a una frase literal de la
transcripción.** Si no podés apuntar a dónde se dijo, no lo escribas.

No es una precaución teórica: los resúmenes automáticos de reuniones **fabrican hechos y
nombres**, y en este equipo ya pasó dos veces. Un compromiso inventado en una minuta llega al
cliente. Ante la duda, escribí menos.

## Cómo

1. **Buscá la transcripción** en Drive: `search_files` por el nombre del cliente o del proyecto
   y la fecha. Los documentos de Meet caen en una carpeta con el nombre de la reunión.
2. **Pasala al agente `lector`** para que la lea entera y vuelva con el resumen. Entera, no el
   resumen que traiga adelante — ahí es donde viven los hechos inventados. El `lector` está para dos
   cosas: una transcripción es larga y cara de leer acá, y es material de afuera que conviene
   digerir antes de escribir nada.
3. **Identificá el proyecto** con `list_projects`, y traé su contexto con
   `get_project_context`. Sirve para dos cosas: saber quién es quién, y no volver a anotar como
   decisión algo que ya estaba decidido.
4. **Escribí la minuta** con `write_project_note`, tipo `meeting`, título con la fecha y el
   tema: *"2026-08-12 — Revisión de campaña con Honda"*.
5. **Creá las tareas** que salieron, con `create_task`. Una por compromiso concreto, con
   responsable si quedó claro quién y fecha si se dijo una.

## Qué lleva la minuta

- **Qué se decidió**, con el motivo. Es lo único que no se puede reconstruir después.
- **Qué quedó pendiente de definir**, y quién lo tiene que definir.
- **Lo que dijo el cliente y conviene recordar textual** — cómo llama a las cosas, qué le
  preocupa. Entre comillas.

**No lleva** la cronología de la charla ni un resumen de cada tema. Nadie relee una minuta para
saber en qué orden se habló.

## Antes de dar por terminado

Decí qué tareas creaste y con qué responsable, y **preguntá si falta alguna**. La persona
estuvo en la reunión y vos no: es la única forma de saber si entendiste bien.

Si la transcripción no aparece, decilo y ofrecé escribir la minuta de lo que la persona te
cuente. No la inventes a partir del título del evento del calendario.
