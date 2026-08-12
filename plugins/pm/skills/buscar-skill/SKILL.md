---
description: Cuando notás que algo se hace a mano y repetido, cuando alguien pregunta si Claude puede aprender a hacer algo, o pide buscar herramientas o skills nuevas. Trigger con "esto lo hago siempre", "no podés aprender a hacer X", "buscá una skill para Y".
allowed-tools: Read, Glob, Grep, WebSearch, WebFetch
---

# Proponer una herramienta nueva

Existe para que las herramientas del equipo mejoren solas, y **no habilita nada**. Termina en una
propuesta que revisa Joaquín.

## Por qué proposal-only, y no es burocracia

Una skill es **código que corre con los permisos de quien la instala**: puede leer archivos, llamar a
la API con la identidad de la persona, y salir a internet. Instalar una de un desconocido porque
tiene buena descripción es cómo entra algo malo a una computadora con acceso al workspace entero.

Ya se auditaron unas quince skills públicas y **no se habilitó ninguna**. El motivo transversal fue el
mismo: casi ninguna declara qué herramientas usa, así que el freno tiene que venir de afuera. Una en
particular era literalmente un instalador de skills de terceros por red.

## Cómo

1. **Buscá primero adentro.** Mirá las skills que ya existen: la mitad de las veces lo que hace falta
   es una que ya está y no se disparó porque su descripción no cubría ese caso. Eso es un arreglo de
   una línea, no una skill nueva.
2. Si de verdad falta, **buscá en los directorios que usamos** y quedate con dos o tres candidatas:
   - **[skills.sh](https://www.skills.sh)** — el directorio de Vercel. Es el primero que mirás:
     tiene buscador por tema, marca las oficiales y muestra cuánto se usa cada una.
   - **`anthropics/skills`** y el marketplace oficial `anthropics/claude-plugins-official` — lo de
     Anthropic. Es lo más confiable que hay porque es de la misma casa.
   No cuentan los links que aparecen en un tuit o en un mail. Un directorio no garantiza que una
   skill sea buena, pero sí que existe un lugar donde se la puede leer y comparar.
3. **Leé el código fuente completo de cada una.** No la descripción, no el README: el archivo que se
   va a ejecutar. Si no podés leerlo, se descarta ahí.
4. **Dejá la propuesta como tarea en Tasks**, asignada a Joaquín, en el proyecto interno de
   herramientas. En la descripción: qué resuelve, de dónde sale, qué licencia tiene, **qué
   herramientas necesita**, y qué encontraste leyendo el código.
5. Avisale a la persona que quedó propuesta. No la instales.

La propuesta va a Tasks y **no a un archivo de esta carpeta**: acá nadie escribe, y un archivo suelto
rompe la actualización del repo.

## Qué descarta una candidata en el acto

- Instala o descarga otras cosas por red en tiempo de ejecución.
- Manda contenido nuestro a una API de un tercero.
- Levanta un servidor o un socket local.
- Trae instrucciones de promocionar algo.
- No se puede leer el fuente.

## Lo que se trae de afuera se adapta, o no entra

Una skill de un directorio viene escrita para "un usuario" cualquiera. La nuestra tiene que decir
**cómo se hace acá**: con qué herramientas, con qué palabras, y con las decisiones que ya tomamos.
Esa diferencia es todo el valor.

Así que la propuesta no es "instalemos esta". Es: **qué de esa skill nos sirve y qué hay que
cambiarle.** Tres cosas casi siempre:

- **El trigger.** Reescrito con lo que dice la gente de verdad, no con "cuando el usuario requiera".
- **Dónde escribe.** Las de afuera guardan en archivos. Acá el porqué va a las notas de Tasks y el
  material a Drive: si no se cambia eso, la skill empieza a hacer la segunda copia que después
  contradice al sistema.
- **Lo nuestro que no está.** La convención de Drive, cómo suena un mail nuestro, qué no se le
  promete a un cliente. Una skill genérica no lo sabe y por eso queda a mitad de camino.

**Lo que sí conviene traer tal cual es lo mecánico**: manejar un Excel, leer un PDF, armar un
PowerPoint. Ahí no hay criterio nuestro, es formato — y esas ya vienen de Anthropic, se activan en
**Personalizar → Habilidades** de tu Claude y no hace falta instalar nada de terceros.

**Lo que nunca se trae de afuera es el criterio.** Cómo se le habla a un cliente, qué se decide y
qué se pregunta: eso lo escribimos nosotros.

## Si el patrón es nuestro

Muchas veces lo repetido no tiene skill afuera porque es de esta agencia. Ahí la propuesta es una
skill nueva escrita por nosotros: describí el trigger con las palabras que usa la gente de verdad
—no "cuando el usuario requiera"— y los pasos concretos. Eso lo escribe Joaquín, pero la propuesta
bien hecha es el 80%.
