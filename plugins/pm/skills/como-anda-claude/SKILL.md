---
description: Cuando la pregunta es sobre Claude mismo y no sobre un proyecto — "¿Claude puede hacer X?", "cómo conecto el Drive", "por qué se olvidó de lo que le dije", "cómo hago para que se acuerde", "esto se puede automatizar", "¿hay una habilidad para Y?", "se me llenó la conversación". También cuando algo de Claude no anda como se espera.
---

# Cómo funciona Claude

**La respuesta va a la documentación oficial, no a la memoria.** Es la única regla de esta skill y
es la que importa.

Lo que un modelo "sabe" sobre Claude tiene fecha de corte y Claude cambia todas las semanas: se
agregan capacidades, cambian las pantallas, se renombran cosas. Contestar de memoria sale bien nueve
de diez veces, y la décima es una instrucción con confianza que manda a la persona a un menú que ya
no existe. Ese error no se siente como error mientras se comete: por eso se mira, no se recuerda.

## Cómo

1. **Buscá en la documentación oficial** antes de contestar:
   - `code.claude.com/docs` — Claude Code: conectores, habilidades, memoria, permisos, plugins.
   - `docs.claude.com` — Claude en general: la app, los planes, los límites.
   - El índice completo de la doc de Claude Code está en `code.claude.com/docs/llms.txt`, que sirve
     para encontrar la página exacta antes de leerla.
2. **Contestá con lo que dice la página**, no con lo que sonaba razonable. Si la doc y tu memoria no
   coinciden, gana la doc.
3. **Traducilo a la pantalla que la persona tiene adelante.** Nada de nombres de archivos ni de
   términos técnicos: "Configuración → Personalizar → Conectores", no una ruta ni un JSON.
4. Si la doc no lo cubre, decí eso: *"la documentación no lo dice; se lo pregunto a Joaquín"*. Es
   mejor que una instrucción inventada, porque la persona la va a seguir.

## Las preguntas que más aparecen

- **"No se acuerda de lo que le dije."** Cada conversación arranca de cero salvo lo que esté escrito
  en algún lado. Lo que tiene que sobrevivir va a las notas del proyecto en Tasks, no a la charla.
- **"Se me llenó la conversación."** `/compact` la resume y sigue; `/clear` arranca limpio y se usa
  al cambiar de tema. Cambiar de tema en la misma conversación es la forma más rápida de que
  responda peor.
- **"¿Puede hacer X?"** Mirá si ya hay una skill del equipo para eso —son las que aparecen con `/`—
  antes de buscar afuera. Si de verdad falta, va por `buscar-skill`, que termina en una propuesta
  para Joaquín y no instala nada.
- **"¿Cómo conecto tal cosa?"** El paso a paso está en `EMPEZA-ACA.md` de esta carpeta, y la doc
  oficial tiene la versión larga.

## Lo que no va

- No inventes menús, botones ni nombres de opciones. Si no lo verificaste, no lo digas.
- No mandes a nadie a la terminal, ni a editar un archivo de configuración, ni a instalar nada. Si
  la solución es eso, es para Joaquín.
- No propongas herramientas de terceros como solución a mano alzada. Una skill de afuera es código
  que corre con los permisos de la persona.
