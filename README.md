# Interact2Hack 2027 · App móvil

Documentos del Avance 2 del proyecto final: el PRD, que define qué se construye, y el sistema de diseño (brand board y DESIGN.md), que define cómo se ve. El proyecto Expo se crea en el Avance 3, a partir de estos documentos.

## Integrantes

- Mateo Montesdeoca
- Nathalia Barriga

## Qué contiene este repositorio

```
README.md                  Este archivo
DESIGN.md                  Sistema de diseño escrito para el agente
docs/
  cliente/
    respuestas.md          Preguntas del Avance 1 con las respuestas del cliente
  prd/
    interact2hack.md       PRD: qué se construye, para quién y con qué reglas
    revision.md            Revisión del PRD: huecos encontrados y cómo se corrigieron
  diseno/
    BRIEF.md               Personalidad, usuarios, sensaciones y qué se toma de cada referencia
    referencias/           5 referencias visuales (una no es una app: el plano isométrico)
    brand-board.html       Sistema de diseño para personas, se abre en el navegador
    Interact2HackAppWireframes.html   Bocetos de las pantallas de la exploración, se abren en el navegador
    marca/                 Logo, ícono de la app y Nooby, tal como los entregó el cliente
    nooby-equipo/          Nooby en pixel art, hecho por el equipo
```

Cómo se relacionan:

1. **[respuestas.md](docs/cliente/respuestas.md)** es la fuente. Cada respuesta tiene un código: P (preguntas), T (prioritarias), N (notas de la sesión) y A (aclaraciones posteriores).
2. **El [PRD](docs/prd/interact2hack.md)** cita esos códigos en cada decisión (D1, D2…). Lo que el cliente no dijo está en Supuestos (S) o en Puntos abiertos (O). **[revision.md](docs/prd/revision.md)** muestra cómo se revisó.
3. **El [BRIEF](docs/diseno/BRIEF.md)** y las referencias explican de dónde salen las decisiones visuales.
4. **El [brand board](docs/diseno/brand-board.html) y [DESIGN.md](DESIGN.md)** describen el mismo sistema, con los mismos tokens: el primero para el equipo y el cliente, el segundo para el agente. En el Avance 3, DESIGN.md se referencia desde AGENTS.md.

**Sobre Nooby:** el cliente entregó el Nooby original (en `marca/`) y dio libertad creativa mientras se respete su diseño. Nathalia lo redibujó en pixel art (`nooby-equipo/nooby-pixel.png`) para el estilo retro de la app; esa es la versión que usan el brand board y los bocetos. El logo y el ícono de la app se extrajeron, sin cambios, del brandboard «Señal Neón» del cliente.

## Cómo abrir el brand board

1. Descarga `docs/diseno/brand-board.html` (o el repositorio completo).
2. Ábrelo con doble clic, o arrástralo a Chrome, Firefox, Edge o Safari.
3. El archivo funciona solo: el logo, el ícono, Nooby, las referencias y la fuente DM Sans van incrustados. Solo las fuentes Bungee y Press Start 2P se cargan desde Google Fonts; sin internet, los títulos y las etiquetas pixel se ven con una fuente del sistema.

En GitHub, el archivo HTML se ve como código. Para ver la página, ábrelo en tu computadora.

## Uso de IA

Usamos Claude (Anthropic) en estas partes. El equipo revisó y aprobó cada resultado antes del commit.

- **Respuestas del cliente:** Claude pasó a Markdown la tabla del Avance 1 con las respuestas anotadas en la sesión. Las aclaraciones posteriores (A1–A25) las dio el equipo después de confirmarlas con el cliente.
- **PRD:** Claude redactó el borrador a partir de `respuestas.md`. Después, siguiendo la guía de la clase, lo revisó como un socio de producto escéptico y encontró huecos (contradicciones, preguntas perdidas, inventos y reglas vagas), anotados en `revision.md` con origen «IA». El equipo respondió cada hueco y Claude aplicó las correcciones. Cada decisión del PRD sale de una respuesta del cliente, citada con su código.
- **Sistema de diseño:** en lugar de Stitch, usamos Claude para explorar la identidad (plan B del taller): a partir del brief, las referencias y el brandboard del cliente, creó los bocetos de las pantallas y los borradores del brand board y de DESIGN.md. El equipo eligió la tipografía, mantuvo las esquinas rectas y limitó el estilo pixel a Nooby y a detalles pequeños. Claude calculó los contrastes de la tabla de colores.
- **Imágenes:** el Nooby en pixel art lo dibujó Nathalia. Claude le quitó el fondo negro, extrajo el logo y el ícono del brandboard del cliente e incrustó las imágenes en el brand board.
- **Repositorio:** Claude Code ayudó a crear la estructura, organizar los archivos, redactar este README y preparar los commits.
