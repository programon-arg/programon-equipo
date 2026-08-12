---
description: Cuando hay que encontrar, guardar u ordenar material de un cliente en Drive — "dónde está el logo de Uiare", "subí esto a la carpeta del cliente", "armá la carpeta de Nadando", "pasame el contrato de Interlatina", "no encuentro la transcripción de la reunión". También antes de crear cualquier carpeta nueva.
---

# El Drive del cliente

Todo el material de clientes vive bajo una sola carpeta: **`Proyectos | Programon`**. Adentro hay
dos niveles y siempre son los mismos.

## La estructura

```
Proyectos | Programon
└── {Cliente} | Cliente              ← la relación con el cliente
    └── {Cliente} | {Proyecto} {año} ← este proyecto puntual
```

- **`{Cliente} | Cliente`** — ejemplo: `Uiare | Cliente`. Acá van los contratos y las propuestas de
  trabajo del equipo, y las subcarpetas de servicio si el cliente es recurrente (`Reuniones`,
  `Propuestas`).
- **`{Cliente} | {Proyecto} {año}`**, anidada adentro — ejemplo: `Uiare | Ecommerce 2026`. Acá van
  los archivos del proyecto en sí: assets de marca, material de referencia, entregables.

El separador es una barra vertical con espacios a los costados, no un guion. Se respeta tal cual
porque es lo que hace que la búsqueda por nombre de cliente traiga todo junto.

**Un cliente puede tener varios proyectos** a lo largo del tiempo, y por eso están separados los dos
niveles: la relación con el cliente de un lado, los archivos de cada proyecto del otro. Mezclarlos
deja una carpeta plana que en un año no se puede leer.

## Antes de crear una carpeta

**Buscá primero si ya existe.** `search_files` por el nombre del cliente. Casi siempre existe y se
está por crear la segunda, que es peor que ninguna: a partir de ahí la mitad del material va a una y
la mitad a la otra.

Si de verdad falta, creá los dos niveles de una: la de cliente y adentro la del proyecto, con el año.

## Para crear un documento

Todo lo que se entrega vive acá y **en formato de Google** — Documento, Presentación, Hoja de
cálculo—, nunca como archivo suelto en la computadora de alguien.

- **Un documento nuevo** se crea directo en la carpeta del proyecto. Mandá el contenido como HTML, no
  como texto pelado: así conserva los títulos, las negritas y las listas en vez de llegar como un
  bloque plano.
- **Un archivo que ya existe** —un PDF que generaste, una planilla— se sube a la carpeta del proyecto
  y se deja **convertir al formato de Google**. Así se puede comentar y no queda una versión muerta.
- **El archivo intermedio** que hizo falta para llegar ahí queda en `Proyectos/<cliente>/` y no se le
  manda a nadie.
- **Editar un documento que ya está en Drive** es lo único que el conector no hace bien. Si hay que
  cambiar algo de fondo, es más limpio crear la versión nueva y decir cuál reemplaza a cuál que
  intentar parcharlo.

Cuando termines, pasá el link y decí en qué carpeta quedó.

## Para encontrar algo

1. `search_files` por nombre de cliente o de proyecto. Los nombres siguen la convención de arriba,
   así que buscar el cliente trae la carpeta y todo lo que cuelga.
2. Las **transcripciones de Meet** no están donde uno espera: Google las guarda en el Drive de quien
   organizó la reunión, en una carpeta con el nombre de la reunión. Buscá por el nombre del evento o
   del cliente y la fecha.
3. Si no aparece, decí que no aparece y ofrecé buscar por otro nombre. No supongas la ubicación.

## Lo que no va

- **No muevas ni borres archivos de un cliente** sin que te lo pidan explícitamente. El material del
  cliente es lo único que no se puede volver a generar.
- No inventes carpetas intermedias porque "quedaría más ordenado". Los dos niveles son la
  convención completa.
- El link de la carpeta va cargado en el proyecto de Tasks con `add_project_link`, así la próxima vez
  no hay que buscarla. Si lo encontraste y no estaba cargado, ofrecé cargarlo.
