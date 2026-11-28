# Brief de diseño · App Interact2Hack 2027

- **Equipo:** Mateo Montesdeoca y Nathalia Barriga
- **Base:** brandboard «Señal Neón» v1.0 entregado por el cliente (P25) y el [PRD](../prd/interact2hack.md).
- **Qué se toma del cliente y qué propone el equipo:** se mantienen el logo, Nooby y la paleta del brandboard, con los roles que el cliente le da a cada color. La tipografía, los componentes y el giro visual de la app los propone el equipo.

## 1. Personalidad

La app es la pantalla encendida en una sala oscura durante el hackatón: informa rápido y sin rodeos, brilla en morado neón y guarda un guiño de videojuego retro en Nooby, que vive en la app como una mascota de bolsillo.

**Tres adjetivos:** nocturna, neón y retro.

| Adjetivo | Qué significa en la app |
| --- | --- |
| Nocturna | Fondo negro en todas las pantallas, como pide el brandboard («el negro manda»). Se lee bien de noche y en salas con poca luz |
| Neón | El morado neón ilumina lo importante y el lima marca un solo dato por pantalla. Nada de colores nuevos: el brillo sale de la paleta del cliente |
| Retro | El giro del equipo: detalles en estilo pixel y de consola portátil, sobre todo en la pestaña «Cuida a Nooby», que se inspira en un Tamagotchi |

## 2. Quién la usa y en qué condiciones

Según las respuestas del cliente:

- **Cualquier persona** que cree una cuenta, inscrita o no en el evento (P2, P5, A1). Entre los usuarios puede haber menores de edad (A11).
- **Durante tres días y 32 horas**, del 19 al 21 de febrero de 2027, en el campus de la USFQ (A13, A24). Se mueve entre la Casa Blanca, el Salón Azul, el patio interno del Da Vinci, el Calderón de la Barca y el Shakespeare (P13).
- **Con internet**: no se pidió que funcione sin conexión (P14).
- **Para consultar rápido** los retos, la agenda y el mapa, que es lo imprescindible (T1), y para **recibir anuncios** aunque tenga la app cerrada (P19).
- **Solo en español** (P28).

Condiciones que el equipo deduce de lo anterior (no las dijo el cliente):

- El evento dura 32 horas, así que la app también se usa de noche y con cansancio.
- Se consulta de pie, caminando entre lugares, muchas veces con una sola mano.

## 3. Qué debe sentir el asistente al abrirla

- **«Ya estoy en el hackatón».** El negro, el morado y el lima son los mismos del evento, la web y las redes.
- **«Sé qué sigue y a dónde ir».** Lo primero que ve es lo que necesita ahora: el último anuncio, lo próximo de la agenda y los retos.
- **«Nooby me está esperando».** Un toque de juego que dan ganas de volver a abrir la app, sin estorbar la información.

## 4. Cómo conviven el logo y Nooby con la propuesta

**Logo del Interact2Hack**

- Se usa tal como lo entregó el cliente, sin recolorear, deformar ni redibujar (brandboard, sección 02).
- Va sobre negro `#050307`, sobre tinta `#0B0612` o sobre foto con el grado morado. Nunca sobre fondos claros.
- Mide al menos 96 px de ancho en la app y respeta su área de protección (X = altura del «2»).
- Aparece en el splash y en el encabezado del Home; no se repite en cada pantalla.

**Nooby**

- El cliente entregó el Nooby original (`marca/`) y dio libertad creativa mientras se respete su diseño (P1, A23).
- El equipo lo redibujó en pixel art (`nooby-equipo/nooby-pixel.png`): es la versión que usa la app y es parte del giro retro. Mantiene la forma, los rasgos y los colores del original.
- Aparece en tres lugares: el splash, la pestaña «Cuida a Nooby» y los estados vacíos o de error.
- El giro retro también vive alrededor de Nooby: un marco tipo consola portátil en forma de huevo, en negro con borde morado neón, y un cuarto en estilo pixel donde vive.
- Nooby nunca tapa información: no aparece encima de tarjetas, anuncios ni retos.

## 5. Referencias visuales

Las imágenes están en `docs/diseno/referencias/`.

| # | Referencia | Tipo | Qué se toma de ella |
| --- | --- | --- | --- |
| 1 | Tamaweb (`01-tamaweb.png`) | Web app | La consola en forma de huevo, el cuarto en pixel art y los tres botones redondos para la pestaña «Cuida a Nooby». Se toma la estructura, no sus colores pastel |
| 2 | Plano urbano isométrico, de Ordinary Mold (`02-mapa-isometrico.png`) | Ilustración de arquitectura (no es una app) | Para el mapa: los edificios en volumen isométrico, las etiquetas en recuadro unidas al edificio con una línea punteada y los íconos redondos que dicen qué hay en cada lugar. Se toma la forma de explicar el plano, no sus colores pastel |
| 3 | App de eventos en modo oscuro (`03-app-eventos-oscura.png`) | App | Tarjetas grandes con foto y el título encima, una insignia con la fecha, la lista de personas con foto y rol, y el ícono activo de la barra inferior en lima, igual que pide el brandboard |
| 4 | App «Adverse» (`04-app-adverse.png`) | App | La fila de fotos redondeadas que se desliza de lado, útil para jueces y mentores; los títulos grandes en mayúsculas sobre la foto, y una pastilla de estado («EN VIVO») para lo que está pasando ahora |
| 5 | Formulario «Create Event» (`05-formulario-crear-evento.png`) | App | Para el panel de admin: un formulario corto con cada campo en su propia fila, una etiqueta clara y un solo botón de acción al final. Se toma el orden del formulario, no su fondo claro ni sus degradados |

**Lo que no se toma de las referencias:** los fondos claros, los degradados de colores y los tonos pastel o naranja. Chocan con la paleta del cliente, que se mantiene (brandboard, secciones 01 y 03).

## 6. Exploración

En lugar de Stitch, usamos Claude para explorar la identidad: a partir de este brief, de las referencias y del brandboard del cliente, propuso los bocetos de las pantallas, el brand board y DESIGN.md, como en el plan B del taller. El equipo eligió la tipografía (Bungee, DM Sans y Press Start 2P), mantuvo las esquinas rectas y limitó el estilo pixel a Nooby y a detalles pequeños. El resultado está en `brand-board.html` y `DESIGN.md`.

## 7. Decisiones tomadas en el brand board

- **Tipografía del equipo:** Bungee para títulos y datos, DM Sans para el texto y Press Start 2P para detalles pixel.
- **Estilo pixel:** en la pestaña «Cuida a Nooby» y en detalles pequeños (pastillas de estado, contadores, carga).
- **Esquinas:** rectas, como pide el brandboard, aunque las referencias 3, 4 y 5 usan esquinas redondeadas.
