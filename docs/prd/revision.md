# Revisión del PRD

Revisión del borrador de `docs/prd/interact2hack.md` contra `docs/cliente/respuestas.md`, con los tipos de hueco de la guía. Origen: **Equipo** (revisión sin IA, paso 2) o **IA** (revisor adversarial, paso 3).

| # | Tipo | Sección | Frase exacta del PRD | Por qué es un problema | Gravedad | Origen | Corrección |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Contradicción | 5 | "D2. Para ver cualquier contenido hay que tener sesión iniciada…" (fuente: A2) | T4 dice «No te bloquea: cualquiera puede ver» y A2 dice que hay que iniciar sesión. El PRD eligió A2 sin decirlo | Alta | IA | Fuente de D2 cambia a «A2 (aclara T4: ver C1)» y se agrega la tabla de contradicciones resueltas (C1) |
| 2 | Contradicción | 3 | "Publica los anuncios desde una página web aparte, con usuario y clave específicos" | T3 dice «Panel de admin, ya existente» y A3 dice que lo construye el equipo. El PRD siguió A3 sin decirlo | Media | IA | Se agrega C2 a la tabla de contradicciones resueltas |
| 3 | Contradicción | 5 | "D6. La app no muestra los perfiles de otros usuarios" | P2 dice «Todas las personas pueden acceder a todo»; A8 lo limita. El PRD siguió A8 sin decirlo | Media | IA | Se agrega C3 a la tabla de contradicciones resueltas |
| 4 | Contradicción | 4 | "Agenda … La administración" | P7 pide un panel tipo formulario para cambiar la agenda; A4 dice que desde el panel se envían los anuncios y el resto va fijo. No está resuelto | Media | IA | Se agrega C4 («sin resolver») y la sección 4 remite a O5 |
| 5 | Pregunta perdida | 9 | (no aparece) | P8 pregunta qué información del jurado se muestra **y desde cuándo**; la respuesta solo cubre el qué | Media | IA | Nuevo punto abierto O11 |
| 6 | Regla vaga | 5 | "D9. Los retos se publican antes del evento…" | «Antes del evento» no se puede comprobar: no dice cuándo. P10 y A5 no dan fecha | Alta | IA | D9 remite a un nuevo punto abierto, O12 (fecha de publicación de los retos) |
| 7 | Pregunta perdida | 9 | (no aparece) | T2 dice «panel de admin no muy complejo, dependiendo los roles»; no está claro si hay varios tipos de admin | Baja | IA | Nuevo punto abierto O13 |
| 8 | Regla vaga | 5 | "D23. … Se puede animar o cambiar de estilo, pero sigue siendo reconocible como el mismo personaje" | «Reconocible» no se puede comprobar, y «animar o cambiar de estilo» salió de nuestra pregunta, no de la respuesta (P1 solo dice «libertad creativa, respetando el diseño») | Media | IA | D23 se reescribe con las palabras de P1 y remite a O14 (qué cambios cuentan como respetar el diseño) |
| 9 | Invento | 4 | "Nooby, respetando su diseño original; se puede animar o adaptar de estilo" | Mismo problema que la fila 8 | Media | IA | Se reescribe con las palabras de P1 y remite a O14 |
| 10 | Invento | 2 | "Campus de la USFQ. Lugares que se usan: …" (fuente: P11, P12, P13) | El cliente no dijo «campus de la USFQ»: eso estaba en nuestra pregunta P11, no en su respuesta. Lo que sí dijo es la lista de lugares (P13) | Baja | IA | La fila dice que el cliente nombró esos lugares para el mapa, con fuente P13 |
| 11 | Invento | 4 | "Perfil … Nombre, correo y foto de perfil" | Ninguna respuesta dice que el perfil muestra el correo. P21 habla de nombre, foto y clave | Baja | IA | El correo pasa a supuesto (S6) |
| 12 | Invento | 7 | "Al eliminar la cuenta se borran esos datos (P21)." | P21 dice que se puede eliminar la cuenta, no qué pasa con los datos. La fuente no respalda la frase | Media | IA | Pasa a supuesto (S7) |
| 13 | Tecnología | 4 | "La organización, en la base de datos de la app" (Retos; Auspiciantes, mentores y jueces) | Dice cómo se construye. Lo que necesita el cliente (P9, A4) es poder cambiarlo sin tocar la app | Baja | IA | Se reescribe: «La organización, sin publicar una nueva versión de la app» |
| 14 | Alcance inflado | 6 y 9 | "S6. Propuesta del equipo: una pestaña «Cuida a Nooby»…" y "S7. El Home muestra … una cuenta regresiva…" | Son funciones que el cliente no pidió. La guía dice que eso va a fuera de alcance o a puntos abiertos, no a supuestos | Alta | IA | Salen de supuestos. Pasan a puntos abiertos como propuestas del equipo (O10 y O16) |
| 15 | Invento | 9 | "S5. Quien olvida su contraseña puede recuperarla por correo." | Nadie le preguntó al cliente qué pasa si se olvida la contraseña | Baja | IA | Sale de supuestos. Pasa a punto abierto (O17) |
| 16 | Alcance inflado | 6 | "Puede esperar al final del proyecto: Anuncios y página web de admin…" | La división entre «imprescindible» y «puede esperar» la hizo el equipo a partir de T1; el cliente no la confirmó, y en el Avance 1 los anuncios tenían prioridad alta | Media | IA | Nota en la sección 6 y nuevo punto abierto O15 |
| 17 | Sección incompleta | 4 | "Agenda … Las mismas actividades para todos los usuarios" y "Retos … Los retos, publicados antes del evento…" | No dicen qué datos muestra cada actividad o reto | Media | IA | La tabla remite a los supuestos S1 y S2 |
| 18 | Sección incompleta | 4 | "Una página por auspiciante, por mentor y por juez…" | Solo dice qué muestran los jueces; no qué muestran mentores y auspiciantes | Media | IA | La tabla remite al punto abierto O9 |
| 19 | Fuente equivocada | 5 | "D12. Al tocar la foto de un juez se abre su página…" (fuente: A6) | A6 no decía que la página se abre al tocar la foto, aunque el cliente sí lo dijo en la aclaración | Baja | IA | Se completa A6 en `respuestas.md` con lo que dijo el cliente |

## Ronda 2 · Respuestas del equipo y del cliente a la revisión

El equipo revisó cada fila con el cliente. Las aclaraciones quedaron en `respuestas.md` (A14–A25) y el PRD pasó a la versión 1.1.

| Fila | Qué se decidió | Fuente nueva | Cómo quedó en el PRD |
| --- | --- | --- | --- |
| 1 | D2 es correcta: hace falta cuenta, no inscripción | — | Se mantiene D2 con C1 |
| 2 | El panel de admin lo arma el equipo: página web aparte, tipo formulario; lo que envía el admin aparece en la app | A14 | Rol de admin, D16 y C2 |
| 3 | Los usuarios no ven perfiles de otros, pero todos ven la misma información | A8 | D5, D6 y C3 |
| 4 | La agenda es fija, no cambia durante el evento; se carga desde el panel | A14, A16 | D8 y C4; O5 resuelto |
| 5 | Del jurado se ve foto, nombre y credenciales, desde siempre | A18 | D12; O11 resuelto |
| 6 | La descripción general de los retos está siempre visible; los detalles se activan desde el panel el día que empieza el hackatón | A17 | D9 y nueva D24; O12 resuelto |
| 7 | Un solo tipo de admin y una sola cuenta | A15 | Nueva D25; O13 resuelto |
| 8 y 9 | Con Nooby se puede hacer cualquier cosa mientras se respete su diseño original | A23 | Splash y D23; O14 resuelto |
| 10 | El evento es en el campus de la USFQ, en los lugares de P13 | A24 | Sección 2 |
| 11 | El correo no se muestra; se editan nombre de usuario, correo y contraseña, nada más | A19 | Perfil y D20; S6 descartado; nueva contradicción C5 |
| 12 | Eliminar la cuenta la desactiva; si vuelve con el mismo correo, se reactiva y se actualizan sus datos | A20 | Nueva D26; S7 descartado; nuevo punto abierto O10 sobre borrado definitivo |
| 13 | Todo se modifica desde el panel, con un formulario por sección | A14 | Sección 4 y D10 |
| 14 | «Cuida a Nooby» y la cuenta regresiva son ideas del equipo, dentro de la libertad creativa que dio el cliente | A25 | Fila «Propuestas del equipo» en la sección 6; O16 resuelto |
| 15 | El cliente confirmó que la contraseña se recupera por correo | A21 | Nueva D27; O17 resuelto |
| 16 | Anuncios, panel, páginas, edición de perfil y reserva de mentorías son imprescindibles; lo importante es saber cuántas personas se registraron | A22 | Sección 6 y métrica principal en la sección 8; O15 resuelto |
| 17 | Todavía no se envían los datos de mentores y auspiciantes | — | O9 sigue abierto |
| 18 | Confirmado: una página por auspiciante, por mentor y por juez | A7 | Sin cambios |
| 19 | Cómo se abre cada página se decide al diseñar la interfaz, no en el PRD | — | D12, D13 y D14 ya no dicen «al tocar»; A6 vuelve a su texto original |

## Para presentar

1.
2.
3.
