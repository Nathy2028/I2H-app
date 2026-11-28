# PRD · App Interact2Hack 2027

- **Versión:** 1.2 · 28 de noviembre de 2026 (revisada con `revision.md`; agrega la propuesta del equipo para las mentorías, S8, y resuelve O18–O21; agrega S9–S11 del panel de admin)
- **Equipo:** Mateo Montesdeoca y Nathalia Barriga
- **Fuente:** [respuestas del cliente](../cliente/respuestas.md). Cada decisión cita de dónde sale: preguntas (P1, P2…), prioritarias (T1…), notas de la sesión (N1…) o aclaraciones posteriores (A1…).

## 1. Resumen

La app del Interact2Hack 2027, que se realiza del 19 al 21 de febrero de 2027 en el campus de la USFQ (A13, A24), es una app informativa (P24, T1) que cualquier persona puede descargar y usar con solo crear una cuenta, aunque no esté inscrita en el evento (P5, A1). Reúne en el teléfono los retos, que se conocen solo dentro de la app (P10, A5); la agenda; un mapa propio de los lugares del evento (P12, P13); las páginas de jueces, mentores y auspiciantes (A6, A7), y los anuncios de la organización, que llegan como notificación aunque la app esté cerrada (P19). La organización maneja todo ese contenido desde un panel web aparte (A14). Lo que el cliente quiere saber al final es cuántas personas se registraron en la app (A22).

## 2. El evento

| Dato | Valor | Fuente |
| --- | --- | --- |
| Fechas | 19, 20 y 21 de febrero de 2027 | A13 |
| Duración | Tres días, 32 horas en total | A13 |
| Lugar | Campus de la USFQ, en los lugares que nombró el cliente: Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare | P13, A24 |
| Asistentes | No se respondió (O1). Como referencia, el brandboard del cliente reporta 247 participantes, 55 equipos, 53 mentores y 19 jurados en la edición 2026 | P25 (brandboard, sección 08) |
| Conectividad | La app funciona con internet; no se pidió que funcione sin conexión | P14 |
| Quién puede usar la app | Cualquier persona, desde cualquier lugar, inscrita o no. El pago de la inscripción se hace fuera de la app | P2, P5, A1 |

## 3. Usuarios y roles

| Rol | Qué ve y qué hace | Fuente |
| --- | --- | --- |
| Usuario (participante o cualquier persona registrada) | Crea una cuenta e inicia sesión. Ve la agenda, los retos, el mapa, los anuncios y las páginas de jueces, mentores y auspiciantes; todos los usuarios ven la misma información. Recibe los anuncios como notificación. Edita su nombre de usuario, su correo y su contraseña, y puede eliminar su cuenta. Puede reservar mentorías | P2, P5, P17, P19, A2, A8, A19 |
| Mentor | Aparece en la app con una página de perfil. Si tiene una cuenta especial en la app está por definir (O4) | P17, T2, A7, A10 |
| Admin (organización) | Hay un solo tipo de admin y una sola cuenta. No administra desde la app móvil: usa un panel web aparte, con usuario y clave, que tiene un formulario por sección (anuncios, retos, agenda, jueces, mentores y auspiciantes). Desde ahí también activa los detalles de los retos el día que empieza el hackatón | P18, P23, T3, A3, A14, A15, A17 |

Los **jueces** y los **auspiciantes** no tienen un rol dentro de la app: solo aparecen en ella, cada uno con su página (T2, A6, A7). La calificación de los proyectos se hace fuera de la app (P22). Los **equipos** se gestionan fuera de la app (N3).

## 4. Secciones de la app

| Sección | Qué hace | Qué muestra | Quién actualiza el contenido | Fuente |
| --- | --- | --- | --- | --- |
| Splash con Nooby | Abre la app con la mascota del evento | Nooby, respetando su diseño original; dentro de eso, el equipo tiene libertad creativa | Fijo | P1, A23 |
| Registro e inicio de sesión | Da acceso a la app a cualquier persona que cree una cuenta | Registro con nombre, correo y contraseña; inicio de sesión con correo y contraseña o con Google (Gmail); recuperación de contraseña por correo | El usuario | P3, P4, P5, N6, A2, A21 |
| Agenda | Muestra las actividades del evento | Las mismas actividades para todos los usuarios, sin separar por reto. La agenda es fija: no cambia durante el evento. Datos de cada actividad: supuesto S1 | El admin, desde el formulario de agenda del panel | P6, A9, A14, A16 |
| Retos | Presenta los retos del evento | Antes del evento, la descripción general de cada reto; desde el día que empieza el hackatón, también sus detalles. Solo se ven en la app. Datos de cada reto: supuesto S2 | El admin, desde el formulario de retos; también activa los detalles | P9, P10, A5, A14, A17 |
| Auspiciantes, mentores y jueces | Muestra quién apoya el evento, quién puede ayudar y quién evalúa | Una página por auspiciante, por mentor y por juez. Jueces: foto, nombre y credenciales, visibles siempre. Mentores y auspiciantes: contenido por definir (O9). Para reservar un horario con un mentor hace falta la clave del evento (propuesta del equipo: S8) | El admin, desde el formulario de cada sección | P8, P16, P17, T2, N1, A6, A7, A14, A18 |
| Mapa | Ayuda a ubicar los lugares del evento | Plano propio con 5 lugares: Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare | Fijo (lo dibuja el equipo) | P12, P13 |
| Anuncios | Comunica avisos de la organización | Los anuncios enviados por el admin, iguales para todos | El admin, desde el formulario de anuncios del panel | P15, P18, P19, A3, A14 |
| Perfil | Muestra y edita los datos del usuario | Nombre de usuario. No muestra el correo, ni equipo, ni reto, ni código QR | El usuario | P20, P21, A19 |

## 5. Reglas de negocio (decisiones del cliente)

| # | Decisión | Fuente |
| --- | --- | --- |
| D1 | Cualquier persona puede crear una cuenta, sin estar inscrita en el evento y sin demostrar un pago | P2, P5, T4, A1 |
| D2 | Para ver cualquier contenido hay que tener sesión iniciada: al abrir la app sin sesión, se muestran el registro y el inicio de sesión | A2 (aclara T4: ver C1) |
| D3 | El registro pide solo nombre, correo y contraseña | P3, T5, A2 |
| D4 | Se puede iniciar sesión con correo y contraseña, o con una cuenta de Google (Gmail) | N6, A2 |
| D5 | Con sesión iniciada, el usuario ve la agenda, los retos, el mapa, los anuncios y las páginas de jueces, mentores y auspiciantes, sin ningún paso adicional. Todos los usuarios ven la misma información | P2, A2, A8 |
| D6 | La app no muestra los perfiles de otros usuarios | A8 |
| D7 | La agenda muestra las mismas actividades a todos los usuarios; no se filtra por reto | P6, A9 |
| D8 | La agenda es fija: no tiene cambios durante el evento. La carga el admin desde el formulario de agenda del panel | P7, A14, A16 |
| D9 | Antes del evento, la app muestra la descripción general de cada reto. Los retos solo se pueden ver dentro de la app móvil | P10, A5, A17 |
| D10 | Los retos, la agenda, los anuncios y las páginas de jueces, mentores y auspiciantes se cargan y se cambian desde el panel web de admin, con un formulario por sección, sin publicar una nueva versión de la app | P9, A4, A14 |
| D11 | El mapa es un plano propio que marca 5 lugares: Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare | P12, P13 |
| D12 | Cada juez tiene una página con su foto, su nombre y sus credenciales (por qué es importante). Las páginas de los jueces se pueden ver desde siempre | P8, N1, A6, A18 |
| D13 | Cada auspiciante tiene su propia página. Los auspiciantes confirmados son NTT DATA, Cursor y Supabase | P16, T2, A7 |
| D14 | Cada mentor tiene su propia página de perfil | P17, A7 |
| D15 | Un usuario puede reservar una mentoría desde la app (mecanismo propuesto por el equipo en S8, pendiente de validar: O4) | P17, A10, A22 |
| D16 | Los anuncios los publica el admin desde el formulario de anuncios de una página web aparte, con usuario y clave. Lo que envía aparece en la app como anuncio. La app móvil no tiene opciones para crear anuncios | P18, P23, T3, A3, A14 |
| D17 | Todos los anuncios llegan a todos los usuarios; no hay anuncios por grupo, reto o rol | P15, N2 |
| D18 | Un anuncio llega como notificación al teléfono aunque la app esté cerrada | P19 |
| D19 | El perfil no muestra equipo, reto ni código QR | P20, N3 |
| D20 | El usuario puede cambiar su nombre de usuario, su correo y su contraseña, y nada más. El perfil no muestra el correo | P21, A19 (ver C5) |
| D21 | La app no recibe calificaciones, votaciones ni puntajes del jurado | P22 |
| D22 | La app incluye términos de uso y una política de privacidad | P27, A11 |
| D23 | Nooby aparece en el splash. El equipo puede presentarlo como quiera (animado, en otro estilo) mientras respete su diseño original | P1, A23 |
| D24 | Los detalles de cada reto aparecen en la app desde el día que empieza el hackatón, cuando el admin los activa desde el panel. Antes de eso solo se ve la descripción general | A15, A17 |
| D25 | Existe un solo tipo de admin y una sola cuenta de admin | A15 |
| D26 | Eliminar la cuenta la deja inactiva, sin borrar sus datos. Si la persona se registra otra vez con el mismo correo, la cuenta vuelve a estar activa con los datos nuevos; no se crea una cuenta nueva | P21, A20 |
| D27 | Quien olvida su contraseña puede recuperarla por correo | A21 |

## 6. Alcance del MVP

| Prioridad | Qué incluye | Fuente |
| --- | --- | --- |
| Imprescindible para el evento | Registro, inicio de sesión y recuperación de contraseña (D1–D4, D27). Retos (D9, D24). Agenda (D7, D8). Mapa (D11). Anuncios (D16–D18). Panel web de admin con sus formularios (D10, D16, D25). Páginas de jueces, mentores y auspiciantes (D12–D14). Edición de perfil y eliminación de cuenta (D20, D26). Reserva de mentorías (D15), con el mecanismo que propone el equipo (S8) | T1, P24, A2, A22 |
| Puede esperar al final del proyecto | Inicio de sesión con GitHub, que el cliente dejó como opcional | A2 |
| Fuera de alcance | Pagos e inscripción al evento (A1). Gestión de equipos (N3). Calificación y votación del jurado (P22). Código QR o check-in (P20). Funcionamiento sin conexión (P14). Idiomas distintos del español (P28). Anuncios por grupo (P15). Perfiles visibles de otros usuarios (A8). Cambios de agenda durante el evento (A16). Varios tipos de admin (A15). Publicación en las tiendas, que hace la universidad (P26) | A1, A8, A15, A16, N3, P14, P15, P20, P22, P26, P28 |
| Propuestas del equipo (dentro de la libertad creativa que dio el cliente) | Pestaña «Cuida a Nooby», tipo Tamagotchi: el usuario alimenta, juega y cuida a Nooby, que se pone triste si no lo atiende. Cuenta regresiva al evento en el Home | P1, A23, A25 |

## 7. Requisitos no funcionales

- **Plataformas:** Android e iOS. La publicación en las tiendas la hace la universidad (P26).
- **Idioma:** solo español (P28).
- **Accesibilidad:** el cliente no pidió requisitos específicos (P28). El equipo aplica los mínimos del curso: contraste de texto de al menos 4,5:1, controles de al menos 44 de alto y estados comunicados con texto, no solo con color.
- **Conexión:** la app funciona con internet; no se requiere funcionamiento sin conexión (P14).
- **Privacidad:** se guardan nombre, correo y contraseña (P3, A19). Eliminar la cuenta no borra los datos: la cuenta queda inactiva y se reactiva si la persona vuelve a registrarse con el mismo correo (A20). La app tiene términos de uso y política de privacidad, y cumple la Ley Orgánica de Protección de Datos Personales del Ecuador, incluido el tratamiento de datos de menores de edad (P27, A11). La retención de datos después del evento está pendiente (O7), igual que cómo se atiende una solicitud de borrado definitivo (O10).
- **Restricción técnica del curso:** la app se construye con React Native, Expo y Firebase (A12).

## 8. Métricas de éxito

| Métrica | Meta | Fuente |
| --- | --- | --- |
| Personas registradas en la app (métrica principal) | Sin meta numérica definida (O8) | P29, A22 |
| Descargas de la app | Sin meta numérica definida (O8) | P29 |

## 9. Supuestos y puntos abiertos

**Supuestos del equipo** (no los dijo el cliente; se confirman antes del Avance 3):

| # | Supuesto | Estado |
| --- | --- | --- |
| S1 | Cada actividad de la agenda muestra hora, nombre y lugar, ordenadas por hora y separadas por día | Vigente |
| S2 | Cada reto muestra su nombre, su categoría, una descripción y quién lo propone | Vigente |
| S3 | Al registrarse, el usuario acepta los términos de uso y la política de privacidad | Vigente |
| S4 | La foto de perfil es opcional | Descartado: A19 dice que solo se editan nombre, correo y contraseña |
| S5 | Las pantallas de ejemplo del brandboard que incluyen «Pase», «Tu equipo» y «Unirme con mi equipo» son ilustrativas (así lo indica el propio brandboard) y no se construyen, porque contradicen P20 y N3 | Vigente |
| S6 | El perfil muestra también el correo del usuario | Descartado: A19 |
| S7 | Al eliminar la cuenta se borran los datos del usuario | Descartado: A20 |
| S8 | Decisión del equipo para las mentorías: el día del evento la organización entrega una sola clave, la misma para todos, que el admin define desde el panel. Solo quien ingresa esa clave en la app puede reservar un horario con un mentor. La clave se ingresa una sola vez: la cuenta queda habilitada y la app no la vuelve a pedir, en ningún teléfono donde se inicie sesión con esa cuenta | Vigente · pendiente de validar con el cliente (O4) |
| S9 | Si el admin cambia la clave de mentorías, las cuentas que ya ingresaron la clave anterior siguen habilitadas | Vigente · decisión del equipo |
| S10 | La clave de mentorías tiene al menos 6 caracteres | Vigente · decisión del equipo |
| S11 | Las actividades de la agenda se ordenan solas por día y hora; el admin no tiene que ordenarlas | Vigente · decisión del equipo |

**Puntos abiertos:**

| # | Pregunta | A quién | Fuente | Estado |
| --- | --- | --- | --- | --- |
| O1 | ¿Cuántos asistentes se esperan en 2027? | Cliente | — | Abierto |
| O2 | ¿Cuáles y cuántos son los retos? | Cliente | P9 | Abierto |
| O3 | ¿Cuál es la lista completa de auspiciantes? ¿Hay niveles de auspicio? | Cliente | P16 | Abierto |
| O4 | ¿Cómo se reserva una mentoría? ¿El mentor tiene una cuenta especial en la app? | Cliente y equipo | P17, A10 | Parcial: el equipo propone la clave del evento (S8); falta que el cliente la valide y definir la cuenta del mentor |
| O5 | ¿La agenda se actualiza desde la página web de admin o igual que los retos? | Cliente | P7, A4 | Resuelto: A14, A16 |
| O6 | ¿Cuándo se entregan los archivos de Nooby? | Cliente | P1, P25 | Abierto |
| O7 | ¿Qué pasa con los datos personales después del evento y cuánto tiempo se guardan? | Organización | P27, A11 | Abierto |
| O8 | ¿Cuántas descargas y registros se considerarían un éxito? | Cliente | P29, A22 | Abierto |
| O9 | ¿Qué información se muestra en la página de cada mentor y de cada auspiciante? | Cliente | P17, T2 | Abierto |
| O10 | Si un usuario pide que se borren sus datos de forma definitiva, ¿cómo se atiende, si eliminar la cuenta solo la desactiva? | Organización | P27, A11, A20 | Abierto |
| O11 | ¿Desde cuándo se puede mostrar la información de los jueces? | Cliente | P8 | Resuelto: A18 |
| O12 | ¿En qué fecha se publican los retos en la app? | Cliente | P10, A5 | Resuelto: A17 |
| O13 | ¿Hay distintos tipos de admin? | Cliente | T2 | Resuelto: A15 |
| O14 | ¿Qué cambios a Nooby cuentan como «respetar su diseño»? | Cliente | P1 | Resuelto: A23 |
| O15 | ¿El cliente está de acuerdo con lo que el equipo puso como imprescindible y como «puede esperar»? | Cliente | T1 | Resuelto: A22 |
| O16 | ¿El cliente aprueba la pestaña «Cuida a Nooby» y la cuenta regresiva? | Cliente | — | Resuelto: A25 |
| O17 | ¿Qué pasa si un usuario olvida su contraseña? | Cliente | — | Resuelto: A21 |
| O18 | ¿La clave de mentorías es una sola para todos o una distinta por persona? | Equipo y cliente | S8 | Resuelto por el equipo: una sola clave para todos (S8) |
| O19 | ¿Quién define la clave de mentorías y desde dónde (por ejemplo, desde el panel de admin)? | Equipo y cliente | S8, A14 | Resuelto por el equipo: el admin, desde el panel (S8) |
| O20 | ¿Qué permite hacer la clave: reservar un horario con un mentor, escribirle o ver sus datos de contacto? | Equipo y cliente | S8, P17 | Resuelto por el equipo: reservar un horario (S8) |
| O21 | Una vez ingresada la clave, ¿queda habilitada la cuenta en cualquier teléfono donde se inicie sesión, o solo en el teléfono donde se ingresó? | Equipo | S8 | Resuelto por el equipo: queda habilitada la cuenta (S8) |

**Contradicciones entre respuestas y cómo se resolvieron:**

| # | Respuesta A | Respuesta B | Qué sigue el PRD |
| --- | --- | --- | --- |
| C1 | T4: «No te bloquea: cualquiera puede ver» | A2: para entrar a la app hay que registrarse e iniciar sesión | A2, que es la aclaración posterior: no se pide inscripción al evento, pero sí una cuenta (D1, D2) |
| C2 | T3: «Panel de admin, ya existente» | A3 y A14: el panel lo construye el equipo, como página web aparte con formularios | A3 y A14 |
| C3 | P2: «Todas las personas pueden acceder a todo» | A8: los perfiles de otros participantes no se muestran | A8: todos ven la misma información, pero no los perfiles de otros usuarios (D5, D6) |
| C4 | P7: los cambios de agenda los hace la administración desde un panel | A4: retos, jueces, mentores y auspiciantes van fijos | A14 y A16: todo se carga desde el panel, y la agenda no cambia durante el evento (D8, D10) |
| C5 | P21: se pueden cambiar «nombre, foto de perfil y clave» | A19: se pueden editar nombre, correo y contraseña, «nada más» | A19, que es la aclaración posterior: no hay foto de perfil (D20) |
