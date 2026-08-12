# Glosario — cómo se llama cada cosa acá

Para que Claude entienda lo que decís sin que se lo expliques cada vez. Lo mantiene Joaquín.

**Esto es vocabulario, no datos.** La lista de clientes, proyectos y quién trabaja en qué **no está
acá**: se pregunta a Tasks (`list_projects`, `list_members`, `get_project_context`), que es lo único
que está al día.

## La agencia

- **Programon** — agencia digital argentina. Founder: Joaquín Berardi.
- Dos verticales: **Growth Studio** (contenido, campañas, growth) y **Development Studio** (sitios,
  ecommerce, sistemas).
- **El sitio** — `programon.co`. De ahí entran los leads.

## Los sistemas

| Cómo le decimos | Qué es |
|---|---|
| **Tasks** | `tasks.programon.co`. Tareas, proyectos, fases, horas y las notas de cada proyecto. Es lo que Claude opera por el conector. |
| **El admin** | `admin.programon.co`. Sistema interno de Joaquín: finanzas, facturación, CRM, sistemas. El equipo no entra. |
| **Una propuesta** | La propuesta comercial de un cliente, publicada en `programon.co/proposals/<cliente>` y protegida con clave. La sube Joaquín. |
| **LaunchKit** | Producto propio (CMO virtual por marca). No es un cliente. |

Tasks y el admin están vinculados: un proyecto puede venir importado del admin, y ahí las horas se
imputan al cliente correcto para facturar. Esa importación se hace desde la pantalla de Tasks, no
desde Claude.

## Las palabras que confunden

- **Proyecto** — en Tasks, un trabajo con fechas y responsables. Un mismo cliente puede tener varios
  a lo largo del tiempo.
- **Fase** — una etapa del roadmap de un proyecto, con fechas. No es una tarea.
- **Nota** — lo que explica algo del proyecto: una decisión, una minuta, el contexto. Vive en Tasks,
  no en un archivo.
- **Contacto** — alguien del lado del cliente. El **principal** es a quien se le pregunta.
- **Bolsa de horas** — horas contratadas por adelantado. Cuando se pasa del umbral, es lo primero
  que hay que decir en un reporte.
- **Cliente** vs **el equipo** — "propuesta al equipo" es lo que se le manda a un freelance nuestro
  para un trabajo; "propuesta" sola es la del cliente. No se mezclan, ni en Drive ni en un mail.

## Drive

Todo el material de clientes cuelga de **`Proyectos | Programon`**, con dos niveles:
`{Cliente} | Cliente` y adentro `{Cliente} | {Proyecto} {año}`. La convención completa está en la
skill `drive`.

## Quién es quién

Los nombres y los roles salen de `list_members` de cada proyecto, que es lo que está al día. Lo único
que conviene tener acá es lo que el sistema no dice:

- **Joaquín** — founder. Decide alcance y precio, y es quien publica las propuestas y las skills.
- **Juan** — growth. No usa Slack: si hay que avisarle algo, es por mail o por WhatsApp.

<!-- Joaquín: completar acá lo que el sistema no puede decir — apodos, quién aprueba qué, con quién
     no se habla directo. Un nombre que ya está en Tasks no hace falta repetirlo. -->
