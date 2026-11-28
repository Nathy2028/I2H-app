# DESIGN.md · App Interact2Hack 2027

Sistema de diseño de la app móvil. Léelo antes de crear o modificar cualquier pantalla, componente o tema.

- **Para personas:** el brand board en `docs/diseno/brand-board.html` muestra este mismo sistema.
- **Qué se construye:** el PRD en `docs/prd/interact2hack.md`. Este documento dice cómo se ve, no qué hace.
- **Base:** brandboard «Señal Neón» v1.0 del cliente. Se mantienen su logo, su paleta, los roles de cada color y las esquinas rectas. El equipo cambia la tipografía y agrega detalles retro en pixel alrededor de Nooby (ver `docs/diseno/BRIEF.md`).
- **Fuente de verdad de los valores (desde el Avance 3):** `src/tema/`. Este documento explica las decisiones.
- **Si algo no está aquí:** no lo inventes. Usa el componente o token más cercano y anota el hueco en «Decisiones pendientes».

## 1. Principios

1. **El negro manda.** Toda pantalla usa `colores.fondo`. No hay modo claro: la app es oscura por diseño, como pide el brandboard.
2. **Una señal por pantalla.** Como máximo un bloque morado sólido (la acción o el aviso principal) y un solo dato en lima (lo que pasa ahora o lo que está activo). Si hay dos, ninguno destaca.
3. **Lo importante, a la vista.** Retos, agenda y mapa son lo imprescindible (PRD, T1): se leen rápido, de pie y de noche, con texto de al menos 14 y áreas táctiles de 48.
4. **Retro alrededor de Nooby, no en todo.** El estilo pixel aparece en la pestaña «Cuida a Nooby» y en detalles pequeños (pastillas de estado, contadores, carga). La información nunca se escribe en pixel.
5. **Esquinas rectas.** Botones, campos y tarjetas sin redondeo. Solo son redondos los avatares, los puntos del mapa, los botones de Nooby y los indicadores.

## 2. Tokens

Se exportarán desde `src/tema/index.ts` como `colores`, `espacio`, `radio`, `texto` y `toque`. Ningún archivo fuera de `src/tema/` escribe un color en hexadecimal ni un tamaño suelto.

### 2.1 Colores

| Token | Valor | Uso | Contraste |
| --- | --- | --- | --- |
| `colores.fondo` | `#050307` | Fondo de todas las pantallas | — |
| `colores.superficie` | `#120B1B` | Tarjetas y campos (morado 8 % sobre negro) | — |
| `colores.tinta` | `#0B0612` | Barra de pestañas; texto sobre `primario` y `acento` | — |
| `colores.borde` | `#28262A` | Borde de tarjetas y separadores (blanco 14 %) | Decorativo |
| `colores.bordeControl` | `#77757A` | Borde de campos y controles | 4,2:1 sobre superficie |
| `colores.texto` | `#FFFFFF` | Texto principal | 20,5:1 sobre fondo · 19,3:1 sobre superficie |
| `colores.textoSuave` | `#A5A4A6` | Texto secundario: lugar, hora, notas (blanco 64 %) | 8,3:1 sobre fondo · 7,8:1 sobre superficie |
| `colores.primario` | `#A46CFB` | Morado neón: acción principal, categorías, enlaces, borde con foco | 6,0:1 sobre fondo · 5,6:1 sobre superficie |
| `colores.sobrePrimario` | `#0B0612` | Texto sobre `primario` | 5,8:1 |
| `colores.primarioProfundo` | `#5B2BB5` | Fondo de avatares con iniciales y decoración | Texto blanco encima: 8,5:1. Nunca como color de texto (2,4:1) |
| `colores.primarioSuave` | `#281A3D` | Fondo de elemento seleccionado; piso del cuarto de Nooby | Texto blanco: 16,1:1 |
| `colores.acento` | `#5CF000` | Lima: un solo dato por pantalla, pestaña activa, «ahora», «abierto» | 13,6:1 sobre fondo |
| `colores.sobreAcento` | `#0B0612` | Texto sobre `acento` | 13,3:1 |
| `colores.exito` / `colores.exitoFondo` | `#3DDC97` / `#0D211B` | Confirmaciones | 9,5:1 |
| `colores.error` / `colores.errorFondo` | `#FF7A7A` / `#281417` | Errores | 6,9:1 |
| `colores.aviso` / `colores.avisoFondo` | `#FFC24B` / `#281E11` | Sin conexión, algo pendiente | 10,2:1 |

Reglas de color:

- `exito`, `error` y `aviso` son semánticos: solo para estados.
- El color nunca es la única señal: cada estado lleva texto y un símbolo (✓, ✕, !, ●).
- El único degradado permitido es el de progreso: de `primario` a `acento`, en barras de carga.
- No se agregan colores fuera de esta tabla.

### 2.2 Espacio

Escala de 4: `espacio.xs` 4 · `espacio.s` 8 · `espacio.m` 12 · `espacio.l` 16 · `espacio.xl` 24 · `espacio.xxl` 32 · `espacio.xxxl` 48.

- Margen lateral de pantalla: `l` (16). Relleno de tarjeta: `l` (16).
- Separación entre tarjetas de una lista: `m` (12). Entre secciones: `xl` (24).

### 2.3 Radio

`radio.ninguno` 0 (botones, campos, tarjetas, pastillas) · `radio.circulo` 999 (avatares, puntos del mapa, botones de Nooby, indicadores).

### 2.4 Texto

Fuentes de Google Fonts (licencia SIL OFL), cargadas con `expo-font`: **Bungee** (títulos y datos), **DM Sans** (texto e interfaz) y **Press Start 2P** (detalles pixel).

| Token | Fuente · tamaño / interlineado | Uso |
| --- | --- | --- |
| `texto.display` | Bungee 400 · 40 / 40 | El dato grande del Home (cuenta regresiva) |
| `texto.titulo` | Bungee 400 · 28 / 30 | Título de pantalla, uno por pantalla |
| `texto.subtitulo` | Bungee 400 · 20 / 24 | Título de sección y nombre de reto |
| `texto.dato` | Bungee 400 · 20 / 20 | Hora de una actividad, cifras |
| `texto.tarjeta` | DM Sans 700 · 16 / 21 | Título de tarjeta |
| `texto.cuerpo` | DM Sans 400 · 16 / 24 | Texto general y campos |
| `texto.nota` | DM Sans 400 · 14 / 20 | Lugar, hora secundaria, ayudas |
| `texto.etiqueta` | DM Sans 700 · 12 / 16 · mayúsculas · espaciado 0,14 em | Categorías, roles |
| `texto.boton` | DM Sans 700 · 15 / 15 | Texto de botones |
| `texto.pestana` | DM Sans 600 · 11 / 14 | Barra de pestañas |
| `texto.pixel` | Press Start 2P 400 · 8 / 12 · mayúsculas | Pastillas de estado, contadores de Nooby |

- Bungee siempre en mayúsculas y nunca por debajo de 20.
- Press Start 2P nunca para párrafos ni para información que solo se diga ahí: lo que dice una pastilla también debe estar en su etiqueta accesible.
- DM Sans respeta el tamaño de texto del sistema; Bungee crece como máximo 1,3×.
- Horas en formato de 24 horas (`09:00`); días con nombre (`Viernes 19`).

### 2.5 Toque

`toque.minimo` 48: alto y ancho mínimos de botones, pestañas, filas y tarjetas tocables. Cubre los 44 que pide el curso y los 48 dp de Android que recomienda el brandboard.

## 3. Componentes

Todos vivirán en `src/components/`, con props en español y estilos que usan solo tokens.

### `Boton`
- Props: `texto`, `alPresionar`, `variante` (`'primario' | 'secundario' | 'texto'`), `deshabilitado?`, `cargando?`, `anchoCompleto?`.
- Primario: fondo `primario`, texto `sobrePrimario`; presionado: fondo `acento`, texto `sobreAcento`. Secundario: borde de 2 en `primario`, texto `texto`. Texto: solo color `primario`. Deshabilitado: fondo `borde`, texto `textoSuave`.
- Esquinas rectas. Alto mínimo `toque.minimo`. `accessibilityRole="button"`; con `cargando`, `accessibilityState={{ busy: true }}`.
- Un solo botón primario por pantalla.

### `CampoTexto`
- Props: `etiqueta`, `valor`, `alCambiar`, `tipo?` (`'texto' | 'correo' | 'contrasena'`), `ayuda?`, `error?`.
- Etiqueta arriba (`texto.etiqueta` sin mayúsculas, DM Sans 700 · 13). Fondo `superficie`, borde 2 en `bordeControl`; con foco, `primario`; con error, borde y mensaje en `error` precedido de «✕».
- La etiqueta se asocia al campo (`accessibilityLabel`); el error se anuncia (`accessibilityLiveRegion="polite"`).

### `BarraPestanas`
- Cinco pestañas: Inicio, Agenda, Retos, Mapa y Nooby. El perfil se abre desde el encabezado del Inicio.
- Fondo `tinta` con línea superior `borde`. Activa: texto `texto`, ícono `acento` y un punto `acento` debajo. Inactiva: `textoSuave`.
- Íconos de línea de 2,4, tamaño 22. Cada pestaña mide al menos `toque.minimo`. `accessibilityRole="tab"` y `accessibilityState={{ selected }}`.

### `EncabezadoPantalla`
- Props: `titulo`, `etiqueta?` (texto pequeño en `primario` encima del título), `alVolver?`, `mostrarPerfil?`.
- Título en `texto.titulo`. Con `mostrarPerfil`, un botón circular de 48 a la derecha que abre el Perfil.

### `Pastilla`
- Props: `texto`, `variante` (`'acento' | 'primario' | 'borde'`).
- Texto en `texto.pixel`. `acento`: «● AHORA», «● DETALLES ABIERTOS». `primario`: «NUEVO». `borde`: estados neutros como «DETALLES EL 19 FEB».
- Siempre con `accessibilityLabel` en texto completo (por ejemplo, «Actividad en curso»).

### `TarjetaActividad`
- Props: `hora`, `titulo`, `lugar`, `ahora?`.
- Hora a la izquierda en `texto.dato`; título (`texto.tarjeta`) y lugar (`texto.nota`) a la derecha. Fondo `superficie`, borde 2 `borde`.
- Con `ahora`: borde `acento` y `Pastilla` «● AHORA».

### `TarjetaReto`
- Props: `categoria`, `titulo`, `descripcion`, `detallesAbiertos`, `alPresionar`.
- Borde superior de 4 en `primario`. Categoría en `texto.etiqueta` color `primario`; título en `texto.subtitulo`; descripción en `texto.nota`.
- `detallesAbiertos = false`: `Pastilla` borde «DETALLES EL 19 FEB» y botón texto «Ver reto». `true`: `Pastilla` acento «● DETALLES ABIERTOS» y «Ver detalles» (PRD, D9 y D24).

### `TarjetaAnuncio`
- Props: `titulo`, `mensaje`, `hora`, `nuevo?`.
- Fondo `superficie`, borde 2 `borde`. Con `nuevo`: borde izquierdo de 6 en `primario` y `Pastilla` primario «NUEVO».

### `TarjetaPersona`
- Props: `tipo` (`'auspiciante' | 'mentor' | 'juez'`), `nombre`, `detalle?`, `imagen?`, `alPresionar`.
- Toda la tarjeta es tocable y abre la página de esa persona o empresa (PRD, D12–D14).
- Auspiciante: logo dentro de un recuadro de 96 × 56 sobre `fondo`. Mentor y juez: foto circular de 56; sin foto, iniciales en `texto.subtitulo` sobre `primarioProfundo`.
- Rol en `texto.etiqueta` color `primario` («AUSPICIANTE», «MENTOR», «JURADO»), nombre en `texto.tarjeta`, detalle en `texto.nota`.

### `FilaAvatares`
- Props: `personas`, `alPresionar`.
- Fila horizontal deslizable de fotos circulares de 64 con el nombre debajo (`texto.nota`). Se usa en el Inicio para jueces y mentores.

### `PuntoMapa`
- Props: `numero`, `nombre`, `seleccionado?`.
- Círculo de 32 con número, fondo `primario` y texto `sobrePrimario`; seleccionado: fondo `acento`. Zona tocable de 48. La etiqueta del lugar va en un recuadro unido al punto por una línea punteada (referencia 2 del brief).

### `ConsolaNooby`
- Props: `estado` (`'feliz' | 'normal' | 'triste'`), `comida`, `diversion`, `cuidado`, `alComer`, `alJugar`, `alCuidar`.
- Huevo en `tinta` con borde 3 `primario` y brillo morado; dentro, un cuarto en pixel con piso `primarioSuave`. Nooby al centro, con el archivo del cliente sin modificar.
- Tres botones circulares de 48 (Comer, Jugar, Cuidar) con su etiqueta en `texto.pixel` y `accessibilityLabel` completo («Darle de comer a Nooby»).
- El estado de Nooby también se dice con texto debajo de la consola: «Nooby está triste. Dale de comer.»

### `EstadoPantalla`
- Props: `tipo` (`'cargando' | 'vacio' | 'error'`), `mensaje`, `accion?`.
- Cargando: texto pixel «CARGANDO…» y barra de 4 con el degradado `primario` → `acento`; `accessibilityRole="progressbar"`.
- Vacío: Nooby de 96 y el mensaje.
- Error: fondo `errorFondo`, borde `error`, mensaje con «✕» y `Boton` secundario «Reintentar»; `accessibilityRole="alert"`.

## 4. Pantallas

| Pantalla | Componentes |
| --- | --- |
| Splash | Nooby y logo centrados sobre `fondo` con brillo morado; barra de carga de `EstadoPantalla`. Sin más texto |
| Registro e inicio de sesión | Logo · `CampoTexto` (nombre, correo, contraseña) · `Boton` primario «Crear cuenta» o «Entrar» · `Boton` secundario «Continuar con Google» · `Boton` texto «¿Olvidaste tu contraseña?» |
| Inicio | `EncabezadoPantalla` con logo y perfil · `TarjetaAnuncio` (el último, con «Ver todos») · cuenta regresiva en `texto.display` · `TarjetaActividad` (próximas) · acceso a `ConsolaNooby` · `FilaAvatares` de jueces y de mentores · `TarjetaPersona` de auspiciantes |
| Agenda | `EncabezadoPantalla` · selector de día con tres `Boton` (Vie 19, Sáb 20, Dom 21; el día elegido en primario) · lista de `TarjetaActividad` ordenada por hora |
| Retos | `EncabezadoPantalla` · lista de `TarjetaReto` · detalle del reto en su propia pantalla |
| Mapa | `EncabezadoPantalla` · plano propio con 5 `PuntoMapa` (Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare) · leyenda numerada debajo |
| Auspiciantes, mentores y jueces | Listas de `TarjetaPersona`. Página de cada uno: foto o logo grande, nombre, rol y datos. En la página del mentor: `CampoTexto` para la clave de mentorías (una sola vez) y la lista de horarios con `Boton` «Reservar horario» |
| Anuncios | `EncabezadoPantalla` con volver · lista de `TarjetaAnuncio`, la más nueva arriba |
| Perfil | `EncabezadoPantalla` con volver · nombre de usuario · `CampoTexto` para editar nombre, correo y contraseña · `Boton` secundario «Cerrar sesión» · `Boton` texto en `error` «Eliminar mi cuenta» |
| Cuida a Nooby | `EncabezadoPantalla` · `ConsolaNooby` · texto del estado de Nooby |

Toda pantalla usa `colores.fondo`, margen lateral 16 y área segura arriba y abajo. Cada pantalla que carga datos usa `EstadoPantalla` para carga, vacío y error.

El panel web de admin queda fuera de este documento: es una página aparte, pero usa los mismos colores, fuentes, `CampoTexto` y `Boton`, con un formulario por sección y un solo botón primario al final (referencia 5 del brief).

## 5. Logo y Nooby

- El logo y el ícono se usan tal como están en `docs/diseno/marca/`: ni recolorear, ni deformar, ni redibujar, ni aplicar filtros.
- El logo va sobre `fondo`, `tinta` o `primarioProfundo`; nunca sobre fondos claros. Mide al menos 96 de ancho y respeta su área de protección (X = altura del «2»).
- El ícono de la app es el monograma del cliente (`marca/icono-app-i2h.png`), sin texto adicional.
- Nooby mide al menos 96 de alto y deja 16 libres alrededor. Va sobre `fondo`, `tinta`, `superficie` o el brillo morado del splash; nunca sobre `acento`, sobre `primario` sólido ni sobre fotos. Aparece en el splash, en «Cuida a Nooby» y en los estados vacíos y de error. Nunca encima de tarjetas, anuncios o retos.
- El estilo pixel del equipo se aplica al entorno de Nooby (consola, cuarto, botones), nunca a su figura.
- La app usa la versión pixel art de Nooby hecha por el equipo (`docs/diseno/nooby-equipo/nooby-pixel.png`), que respeta el diseño original del cliente (`docs/diseno/marca/`) dentro de la libertad creativa que dio (PRD, P1 y A23). No se redibuja ni se recolorea más.
- Se escala sin suavizado, en múltiplos enteros cuando se pueda, para que los píxeles queden nítidos.

## 6. Voz y textos

- Tuteo, frases cortas, verbo primero: «Busca el Salón Azul en el mapa.»
- Un error dice qué pasó y qué hacer: «Esa clave no es la del evento. Revísala e inténtalo otra vez.»
- Los vacíos acompañan: «Todavía no hay anuncios. Te avisamos cuando haya novedades.»
- Botones con la acción exacta: «Reservar horario», «Ver en el mapa». Nunca «Aceptar».
- Fechas como «19–21 de febrero»; horas en 24 horas.
- Sin exageraciones ni afirmaciones sin fuente («el mejor hackatón del país»).
- Todo en español (PRD, P28).

## 7. Accesibilidad

- Contraste mínimo 4,5:1 para texto y 3:1 para bordes de controles; la tabla de colores ya lo cumple.
- Todo control mide al menos 48 × 48, tiene `accessibilityRole` y una etiqueta que se entiende sin ver la pantalla.
- «Ahora», «Nuevo», «Detalles abiertos» y los estados se dicen con texto, no solo con color.
- Lo que se muestra en Press Start 2P también está en su etiqueta accesible.
- Con «reducir movimiento» activado, Nooby y las transiciones aparecen sin animación.

## 8. Sí y no

| Sí | No |
| --- | --- |
| Fondo negro en todas las pantallas | Fondos claros o un modo claro |
| Un bloque morado y un dato lima por pantalla | Varios botones primarios o varios datos en lima |
| Texto `sobrePrimario` (tinta) sobre morado | Texto blanco sobre morado neón (3,4:1) |
| Esquinas rectas en botones, campos y tarjetas | Tarjetas o botones redondeados |
| Bordes de 2 para separar tarjetas | Sombras, o degradados fuera de la barra de progreso |
| «● AHORA» en la actividad en curso | Una actividad resaltada solo con color |
| Pixel en pastillas, contadores y la consola de Nooby | Párrafos o títulos de información en Press Start 2P |
| Nooby en el splash, en su pestaña y en los vacíos | Nooby decorando tarjetas o encabezados |
| Reutilizar `Boton` y las tarjetas | Un `Pressable` con estilos nuevos en cada pantalla |

## 9. Decisiones pendientes

- Sprites de Nooby para sus estados (feliz, normal, triste) en la consola; por ahora hay un solo sprite.
- Contenido de las páginas de mentores y auspiciantes (PRD, O9).
- Si hay niveles de auspicio y cómo cambian el tamaño de los logos (PRD, O3).
- Diseño del plano del mapa: posición de cada lugar en el campus.
- Íconos de los cinco lugares del mapa.
- Diseño del panel web de admin.
