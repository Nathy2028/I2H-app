# PRD · App Interact2Hack 2027

- **Versión:** 1.0 · 24 de noviembre de 2026
- **Equipo:** Mateo Montesdeoca y Nathalia Barriga
- **Fuente:** [respuestas del cliente](../cliente/respuestas.md). Cada decisión cita de dónde sale: preguntas (P1, P2…), prioritarias (T1…), notas de la sesión (N1…) o aclaraciones posteriores (A1…).

## 1. Resumen

La app del Interact2Hack 2027, que se realiza del 19 al 21 de febrero de 2027 (A13), es una app informativa (P24, T1) que cualquier persona puede descargar y usar con solo crear una cuenta, aunque no esté inscrita en el evento (P5, A1). Reúne en el teléfono lo que un asistente necesita para el hackatón: los retos, que se revelan antes del evento y solo dentro de la app (P10, A5); la agenda; un mapa propio de los lugares del evento en el campus (P12, P13); las páginas de jueces, mentores y auspiciantes (A6, A7), y los anuncios de la organización, que llegan como notificación aunque la app esté cerrada (P19).

## 2. El evento

| Dato | Valor | Fuente |
| --- | --- | --- |
| Fechas | 19, 20 y 21 de febrero de 2027 | A13 |
| Duración | Tres días, 32 horas en total | A13 |
| Lugar | Campus de la USFQ. Lugares que se usan: Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare | P11, P12, P13 |
| Asistentes | No se respondió en la sesión. Ver punto abierto O1. Como referencia, el brandboard del cliente reporta 247 participantes, 55 equipos, 53 mentores y 19 jurados en la edición 2026 | P25 (brandboard, sección 08) |
| Conectividad | La app funciona con internet; no se pidió que funcione sin conexión | P14 |
| Quién puede usar la app | Cualquier persona, desde cualquier lugar, inscrita o no. El pago de la inscripción se hace fuera de la app | P2, P5, A1 |

## 3. Usuarios y roles

| Rol | Qué ve y qué hace en la app | Fuente |
| --- | --- | --- |
| Usuario (participante o cualquier persona registrada) | Crea una cuenta e inicia sesión. Ve la agenda, los retos, el mapa, los anuncios y las páginas de jueces, mentores y auspiciantes. Recibe los anuncios como notificación. Edita su nombre, foto de perfil y contraseña, y puede eliminar su cuenta. Puede reservar mentorías | P2, P5, P17, P19, P21, A2, A8 |
| Mentor | Aparece en la app con una página de perfil que los usuarios pueden ver. Si tiene una cuenta especial en la app está por definir (O4) | P17, T2, A7, A10 |
| Admin (organización) | No usa la app móvil para administrar. Publica los anuncios desde una página web aparte, con usuario y clave específicos. La administración hace los cambios de agenda | P7, P18, P23, T3, A3 |

Los **jueces** y los **auspiciantes** no tienen un rol dentro de la app: solo aparecen en ella, cada uno con su página (T2, A6, A7). La calificación de los proyectos se hace fuera de la app (P22). Los **equipos** se gestionan fuera de la app (N3).

## 4. Secciones de la app

| Sección | Qué hace | Qué muestra | Quién actualiza el contenido | Fuente |
| --- | --- | --- | --- | --- |
| Splash con Nooby | Abre la app con la mascota del evento | Nooby, respetando su diseño original; se puede animar o adaptar de estilo | Fijo | P1 |
| Registro e inicio de sesión | Da acceso a la app a cualquier persona que cree una cuenta | Registro con nombre, correo y contraseña; inicio de sesión con correo y contraseña o con Google (Gmail) | El usuario, al registrarse | P3, P4, P5, N6, A2 |
| Agenda | Muestra las actividades del evento | Las mismas actividades para todos los usuarios, sin separar por reto | La administración | P6, P7, A9 |
| Retos | Presenta los retos del evento | Los retos, publicados antes del evento y visibles solo en la app | La organización, en la base de datos de la app | P9, P10, A4, A5 |
| Mapa | Ayuda a ubicar los lugares del evento | Plano propio con 5 lugares: Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare | Fijo (lo dibuja el equipo) | P11, P12, P13 |
| Auspiciantes, mentores y jueces | Muestra quién apoya el evento, quién puede ayudar y quién evalúa | Una página por auspiciante, por mentor y por juez, que se abre al tocar su logo o foto. Jueces: nombre, foto y credenciales | La organización, en la base de datos de la app | P8, P16, P17, T2, N1, A4, A6, A7 |
| Anuncios | Comunica avisos de la organización | Los anuncios enviados por el admin, iguales para todos | El admin, desde la página web aparte | P15, P18, P19, A3 |
| Perfil | Muestra y edita los datos del usuario | Nombre, correo y foto de perfil. Sin equipo, sin reto y sin código QR | El usuario | P20, P21 |

## 5. Reglas de negocio (decisiones del cliente)

| # | Decisión | Fuente |
| --- | --- | --- |
| D1 | Cualquier persona puede crear una cuenta, sin estar inscrita en el evento y sin demostrar un pago | P2, P5, T4, A1 |
| D2 | Para ver cualquier contenido hay que tener sesión iniciada: al abrir la app sin sesión, se muestran el registro y el inicio de sesión | A2 |
| D3 | El registro pide solo nombre, correo y contraseña | P3, T5, A2 |
| D4 | Se puede iniciar sesión con correo y contraseña, o con una cuenta de Google (Gmail) | N6, A2 |
| D5 | Con sesión iniciada, el usuario ve la agenda, los retos, el mapa, los anuncios y las páginas de jueces, mentores y auspiciantes, sin ningún paso adicional | P2, A2, A8 |
| D6 | La app no muestra los perfiles de otros usuarios | A8 |
| D7 | La agenda muestra las mismas actividades a todos los usuarios; no se filtra por reto | P6, A9 |
| D8 | Un cambio en la agenda hecho por la administración se ve en la app sin publicar una nueva versión ni reinstalarla | P7, T3 |
| D9 | Los retos se publican antes del evento y solo se pueden ver dentro de la app móvil | P10, A5 |
| D10 | Los retos y las páginas de jueces, mentores y auspiciantes se pueden cambiar sin publicar una nueva versión de la app | P9, A4 |
| D11 | El mapa es un plano propio que marca 5 lugares: Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare | P12, P13 |
| D12 | Al tocar la foto de un juez se abre su página, con su nombre, su foto y sus credenciales | P8, N1, A6 |
| D13 | Al tocar el logo de un auspiciante se abre su página. Los auspiciantes confirmados son NTT DATA, Cursor y Supabase | P16, T2, A7 |
| D14 | Al tocar la foto de un mentor se abre su página de perfil | P17, A7 |
| D15 | Un usuario puede reservar una mentoría desde la app (el mecanismo está pendiente: O4) | P17, A10 |
| D16 | Los anuncios los publica un admin desde una página web aparte, con usuario y clave; la app móvil no tiene opciones para crear anuncios | P18, P23, T3, A3 |
| D17 | Todos los anuncios llegan a todos los usuarios; no hay anuncios por grupo, reto o rol | P15, N2 |
| D18 | Un anuncio llega como notificación al teléfono aunque la app esté cerrada | P19 |
| D19 | El perfil no muestra equipo, reto ni código QR | P20, N3 |
| D20 | El usuario puede cambiar su nombre, su foto de perfil y su contraseña, y puede eliminar su cuenta | P21 |
| D21 | La app no recibe calificaciones, votaciones ni puntajes del jurado | P22 |
| D22 | La app incluye términos de uso y una política de privacidad | P27, A11 |
| D23 | Nooby aparece con su diseño original. Se puede animar o cambiar de estilo, pero sigue siendo reconocible como el mismo personaje | P1 |

## 6. Alcance del MVP

| Prioridad | Qué incluye | Fuente |
| --- | --- | --- |
| Imprescindible para el evento | Registro e inicio de sesión, porque sin sesión no se ve nada (D1–D4). Retos (D9, D10). Agenda (D7, D8). Mapa (D11) | T1, P24, A2 |
| Puede esperar al final del proyecto | Anuncios y página web de admin (D16–D18). Páginas de jueces, mentores y auspiciantes (D12–D14). Edición de perfil y eliminación de cuenta (D20). Reserva de mentorías (D15), cuando se defina el mecanismo. Inicio de sesión con GitHub (opcional según A2) | T1, P24, A2 |
| Fuera de alcance | Pagos e inscripción al evento (A1). Gestión de equipos (N3). Calificación y votación del jurado (P22). Código QR o check-in (P20). Funcionamiento sin conexión (P14). Idiomas distintos del español (P28). Anuncios por grupo (P15). Perfiles visibles de otros usuarios (A8). Publicación en las tiendas, que hace la universidad (P26) | A1, N3, P14, P15, P20, P22, P26, P28, A8 |

**Propuesta del equipo, pendiente de validar con el cliente:** la pestaña «Cuida a Nooby» (supuesto S6). No forma parte del MVP hasta que el cliente la apruebe.

## 7. Requisitos no funcionales

- **Plataformas:** Android e iOS. La publicación en las tiendas la hace la universidad (P26).
- **Idioma:** solo español (P28).
- **Accesibilidad:** el cliente no pidió requisitos específicos (P28). El equipo aplica los mínimos del curso: contraste de texto de al menos 4,5:1, controles de al menos 44 de alto y estados comunicados con texto, no solo con color.
- **Conexión:** la app funciona con internet; no se requiere funcionamiento sin conexión (P14).
- **Privacidad:** solo se guardan nombre, correo, contraseña y foto de perfil (P3, P21). Al eliminar la cuenta se borran esos datos (P21). La app tiene términos de uso y política de privacidad, y cumple la Ley Orgánica de Protección de Datos Personales del Ecuador, incluido el tratamiento de datos de menores de edad (P27, A11). La retención de datos después del evento está pendiente (O7).
- **Restricción técnica del curso:** la app se construye con React Native, Expo y Firebase (A12).

## 8. Métricas de éxito

| Métrica | Meta | Fuente |
| --- | --- | --- |
| Descargas de la app | Sin meta numérica definida (O8) | P29 |
| Usuarios registrados | Sin meta numérica definida (O8) | P29 |

## 9. Supuestos y puntos abiertos

**Supuestos del equipo** (no los dijo el cliente; se confirman antes del Avance 3):

- S1. Cada actividad de la agenda muestra hora, nombre y lugar, ordenadas por hora y separadas por día.
- S2. Cada reto muestra su nombre, su categoría, una descripción y quién lo propone.
- S3. Al registrarse, el usuario acepta los términos de uso y la política de privacidad.
- S4. La foto de perfil es opcional.
- S5. Quien olvida su contraseña puede recuperarla por correo.
- S6. Propuesta del equipo: una pestaña «Cuida a Nooby», tipo Tamagotchi, donde el usuario alimenta, juega y cuida a Nooby, que se pone triste si no lo atiende. Su objetivo es que la gente vuelva a abrir la app.
- S7. El Home muestra el último anuncio, una cuenta regresiva al evento, lo próximo de la agenda y accesos a jueces, mentores y auspiciantes.
- S8. Las pantallas de ejemplo del brandboard que incluyen «Pase», «Tu equipo» y «Unirme con mi equipo» son ilustrativas (así lo indica el propio brandboard) y no se construyen, porque contradicen P20 y N3.

**Puntos abiertos:**

| # | Pregunta | A quién | Fuente |
| --- | --- | --- | --- |
| O1 | ¿Cuántos asistentes se esperan en 2027? | Cliente | — |
| O2 | ¿Cuáles y cuántos son los retos? | Cliente | P9 |
| O3 | ¿Cuál es la lista completa de auspiciantes? ¿Hay niveles de auspicio? | Cliente | P16 |
| O4 | ¿Cómo se reserva una mentoría? ¿El mentor tiene una cuenta especial en la app? | Cliente y equipo | P17, A10 |
| O5 | ¿La agenda se actualiza desde la página web de admin o directamente en la base de datos? | Cliente | P7, A4 |
| O6 | ¿Cuándo se entregan los archivos de Nooby? | Cliente | P1, P25 |
| O7 | ¿Qué pasa con los datos personales después del evento y cuánto tiempo se guardan? | Organización | P27, A11 |
| O8 | ¿Cuántas descargas y registros se considerarían un éxito? | Cliente | P29 |
| O9 | ¿Qué información se muestra en la página de cada mentor y de cada auspiciante? | Cliente | P17, T2 |
| O10 | ¿Se aprueba la pestaña «Cuida a Nooby» (S6)? Si se aprueba, ¿el usuario recibe una notificación cuando Nooby está triste? | Cliente | S6 |
