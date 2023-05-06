Punto de partida

Cuando queremos recuperar una contraseña hago una peticion que me pide el email

/api/v1/auth/recovery-password
- post crear un nuevo recovery password
    - Llegar el correo electronico 
    - Link que te permite hacer una peticion para actualizar tus datos

/api/v1/auth/recovery-password/:id
- patch actualizar la contraseña validando el enlace del recovery password
    - cuando mandamos la nueva contraseña pasan 2 cosas
        - Se modifica la contraseña en el usuario
        - Se modifica el recoveryToken como ya usado, para que no se pueda volver a utilizar

OPCIONAL: Debera mostrar las conversaciones del usuario loggeado
Retos Opcionales
a. /api/v1/conversations/:conversation_id/participants i. Esta ruta debe estar protegida ii. Mostrara los participantes de la conversacion iii. Permitira agregar nuevos participantes a la conversacion

b. /api/v1/conversations/:conversation_id/participants/:participant_id i. Esta ruta debe estar protegida ii. Mostrara un participante en especifico de la conversacion iii. Permitira eliminar participantes de la conversacion



