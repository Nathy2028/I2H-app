# Respuestas del cliente · Interact2Hack 2027

- **Sesión con el cliente:** jueves 19 de noviembre de 2026, en clase.
- **Equipo:** Mateo Montesdeoca y Nathalia Barriga.
- **Fuente:** documento del Avance 1 con las respuestas anotadas durante la sesión. La sección 3 recoge aclaraciones que el equipo anotó después, para respuestas cortas o ambiguas.
- **Cómo se usa:** cada decisión del PRD cita de dónde sale: una pregunta (P1, P2…), una de las cinco prioritarias (T1…), una nota de la sesión (N1…) o una aclaración (A1…).

## 1. Tabla de preguntas

| # | Sección o área | Pregunta | Prioridad | Respuesta del cliente |
| --- | --- | --- | --- | --- |
| P1 | Splash con Nooby | ¿Qué libertad tenemos con Nooby: usarlo tal cual, adaptarlo a otro estilo o animarlo? | Media | Libertad creativa, respetando el diseño de Nooby. |
| P2 | Registro / Usuarios y roles | ¿Quiénes son las personas que pueden acceder? | Alta | Todas las personas pueden acceder a todo. |
| P3 | Registro | ¿Qué datos de cada participante necesita la organización? | Alta | Nombre y correo para el registro, nada más. |
| P4 | Registro | ¿La cuenta ya existe al inscribirse o se crea en la app? | Alta | No existe; se tiene que crear con el registro de la app. |
| P5 | Registro | ¿Puede usar la app alguien que no esté inscrito en el evento? | Alta | Sí. Con crear una cuenta en la app ya puede acceder. |
| P6 | Agenda | ¿Qué actividades son obligatorias y cuáles opcionales, o se separan por reto? | Alta | Todo llega a todos. |
| P7 | Agenda | ¿Quién hace los cambios de agenda durante el evento? | Alta | La administración. Debe haber un panel de admin aparte, tipo formulario. |
| P8 | Retos | ¿Qué información del jurado se puede mostrar y desde cuándo? | Media | Credenciales, foto y nombre. |
| P9 | Retos | ¿Cuántos retos hay? | Media | Nos lo van a enviar. Debe estar en una base de datos, no quemado en el código. |
| P10 | Retos | ¿Los retos se revelan en un momento específico o están siempre disponibles? | Media | Antes del evento, solo en la app móvil. |
| P11 | Mapa interactivo | ¿Es la típica imagen del mapa de la USFQ? | Baja | Se responde en P12. |
| P12 | Mapa interactivo | ¿Nos van a dar el mapa o tenemos que dibujarlo nosotros? | Media | Vamos a hacer nuestro propio mapa. |
| P13 | Mapa interactivo | ¿Qué lugares debe marcar el mapa? | Media | Casa Blanca, Salón Azul, patio interno del Da Vinci, Calderón de la Barca y Shakespeare. |
| P14 | Mapa interactivo | ¿Tiene que funcionar sin internet? | Media | No es necesario. |
| P15 | Auspiciantes y mentores | ¿A qué grupos necesitan mandar avisos distintos (todos, un reto, mentores, jueces)? | Media | Anuncios generales: los anuncios son para todos. |
| P16 | Auspiciantes y mentores | ¿Cuántos auspiciantes hay? | Baja | NTT DATA, Cursor y Supabase. Nos van a enviar los demás. |
| P17 | Auspiciantes y mentores | ¿Se puede pedir o agendar una mentoría desde la app? | Media | Se pueden reservar mentorías y ver el perfil de los mentores. (Aún no está definido cómo se hará.) |
| P18 | Anuncios | ¿Quién de la organización publica los anuncios? | Alta | Un usuario admin, a través del panel aparte. |
| P19 | Anuncios | ¿Los anuncios deben llegar aunque la app esté cerrada? | Alta | Sí, deben llegar como notificaciones push. |
| P20 | Perfil | ¿El perfil muestra equipo, reto elegido y un código QR para el check-in? | Media | No. |
| P21 | Perfil | ¿Qué datos se pueden editar y cuáles no? | Baja | Puedes eliminar tu cuenta y cambiar tus datos, como nombre, foto de perfil y clave. |
| P22 | Usuarios y roles | ¿Cómo califica hoy el jurado los proyectos? ¿La votación es secreta y se revela al final? | Media | Externo; la app no tiene nada que ver ahí. |
| P23 | Contenido y administración | ¿Desde dónde quieren actualizar la información: computadora, celular o ambos? | Alta | Desde una página web. |
| P24 | El evento | ¿Qué funcionalidad considerarías la más importante? | Alta | Ver los retos y entenderlos, que la agenda y el mapa estén claros. Es una app informativa. |
| P25 | Identidad visual | ¿Qué material de marca nos pueden dar (logo, colores, tipografías, Nooby)? | Media | Nos van a enviar una página con toda la identidad visual. (Entregada: brandboard «Señal Neón» v1.0.) |
| P26 | Plataformas y publicación | ¿En qué sistema operativo se va a publicar la app? | Alta | Ambas. La publicación la hace la universidad; el equipo no tiene que ocuparse de eso. |
| P27 | Datos y privacidad | ¿Qué datos de los participantes puede guardar la app y por cuánto tiempo? ¿Cómo manejan hoy la autorización de los menores de edad? | Alta | Sí, hay que hacer términos de uso y política de privacidad. |
| P28 | Idioma y accesibilidad | ¿Qué factores de accesibilidad se deben tomar en cuenta, como idiomas, accesibilidad, entre otros? | Baja | No importa. Español. |
| P29 | Éxito | ¿Cómo sabrán que la app funcionó (descargas, uso durante el evento, menos preguntas a los organizadores)? | Media | Descargas y registros. |

## 2. Las 5 prioritarias (respuestas de la sesión)

| # | Pregunta | Respuesta del cliente |
| --- | --- | --- |
| T1 | ¿Qué es imprescindible que funcione el día del evento? | Ver los retos y entenderlos, que la agenda y el mapa estén claros. Es una app informativa. |
| T2 | ¿Quiénes usan la app y qué puede hacer cada rol? | Participantes, mentores y admin. Panel de admin no muy complejo, según los roles. Auspiciantes: visibilidad, una mini página por auspiciante. Nada específico para los jueces, solo el mapa. |
| T3 | ¿Quién carga y actualiza agenda, retos y anuncios, y desde dónde? | Panel de admin, con usuario y clave específicos, en tiempo real. |
| T4 | ¿Cómo se crea y valida la cuenta? | No te bloquea: cualquiera puede ver. No es necesario inscribirse en el evento. |
| T5 | ¿Qué datos de cada participante necesita la organización? | Nombre y correo. |

### Notas sueltas de la sesión

| # | Nota |
| --- | --- |
| N1 | Mostrar quiénes van a ser los jueces. |
| N2 | Los anuncios son generales, para todos. |
| N3 | Los equipos se gestionan fuera de la app. |
| N4 | El perfil está abierto. |
| N5 | La vista de admin puede ser web, no en la app. Carga retos y anuncios. |
| N6 | Registro e inicio de sesión con Google, GitHub o correo. |
| N7 | Firebase. |

## 3. Aclaraciones posteriores a la sesión

Puntos que el equipo aclaró con el cliente después de la sesión.

| # | Tema | Aclaración | Aclara a |
| --- | --- | --- | --- |
| A1 | Acceso | La app se puede descargar desde cualquier lugar, sin estar inscrito en el evento. El pago de la inscripción se hace fuera de la app. | P2, P5, T4 |
| A2 | Inicio de sesión | Para entrar a la app hay que registrarse e iniciar sesión. Con eso se ve todo: no hay que demostrar inscripción ni pago. Lo importante es correo con contraseña y Gmail; GitHub es opcional. | P4, P5, T4, N6 |
| A3 | Panel de admin | Lo construye el equipo; no existe uno previo. Es una página web aparte, tipo formulario, desde la que el admin envía anuncios (por ejemplo: «Chicos, nos vemos en 20 minutos en X lugar») que llegan a los teléfonos de todos. | P7, P18, P23, T3, N5 |
| A4 | Contenido fijo | Retos, jueces, auspiciantes y mentores van fijos, pero guardados en la base de datos para poder editarlos fácilmente sin cambiar el código. Desde el panel de admin se envían los anuncios. | P9, P23, T3 |
| A5 | Retos | Se revelan antes del evento y solo en la app, para que haya una razón para descargarla. | P10 |
| A6 | Jueces | Cada juez tiene su página: nombre, quién es y sus credenciales (por ejemplo, «dueño de una empresa»). | P8, N1 |
| A7 | Auspiciantes y mentores | Cada auspiciante y cada mentor tiene su página, que se abre al tocar su foto o logo. | P16, P17, T2 |
| A8 | Qué es público | «El perfil está abierto» significa que cualquier usuario con sesión ve las páginas de mentores, jueces, auspiciantes, retos y anuncios. Los perfiles de otros participantes no se muestran. Ese contenido no lo edita ningún usuario de la app. | N4 |
| A9 | Agenda | Todas las actividades y notificaciones llegan a todos, sin importar el reto del participante. | P6, P15 |
| A10 | Mentorías | El cliente no definió cómo se reservan ni si el mentor tiene una cuenta especial. | P17, T2 |
| A11 | Privacidad | Además de términos de uso y política de privacidad, hay que cumplir la ley ecuatoriana sobre datos de menores de edad. | P27 |
| A12 | Tecnología | Se puede usar Firebase si el equipo quiere. | N7 |
| A13 | Fechas y duración | El evento es el 19, 20 y 21 de febrero de 2027: tres días, 32 horas en total. No se preguntó en la sesión; coincide con las fechas del brandboard. | P25 |

## 4. Material entregado por el cliente

| Material | Estado |
| --- | --- |
| Brandboard «Señal Neón» v1.0 (colores, tipografía, componentes, app móvil) | Entregado |
| Logos del Interact2Hack, USFQ Medios Interactivos y NESTLab (versiones blancas) | Entregados dentro del brandboard |
| Archivos de Nooby | Pendiente |
| Lista de retos | Pendiente (P9) |
| Lista completa de auspiciantes | Pendiente (P16) |
