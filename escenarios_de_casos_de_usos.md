# Escenarios de casos de uso

## Caso 1: Notificaciones

### Descripcion general:
 - El sistema notifica al paciente sobre su turno confirmado de manera automatica cuando el usuario realiza el pago, proporcionando un mail con la fecha y medico designado a modo de recordatorio.

### Flujo de eventos
 - El sistema recopila la informacion del turno.

 - El sistema redacta un mail con la informacion necesaria sobre el turno.

 - El sistema envia la notificacion al correo de usuario.

### Precondiciones

 - El usuario debe estar registrado en el sistema.
 - El usuario debe haber proporcionado un medio de contacto (correo electrónico, número de teléfono, etc.).
 - El turno debe estar programado y confirmado.

### Poscondiciones 

 - El usuario recibe una notificación sobre su turno.
 - Se registra la fecha y hora de la notificación en el sistema.

