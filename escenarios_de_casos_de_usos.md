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


![caso1](https://github.com/user-attachments/assets/d3624156-684d-484a-88e5-fea32b4a066f)



## Caso 2: Cambio de turno

### Descripcion general

 - El usuario puede realizar cambios en el turno pedido ingresando al sistema y dirigiendose a "solicitar cambio de turno".

### Flujo de eventos

 - El usuario ingresa a sistema.

 - El usuario se dirige a "solicitar cambio de turno".

 - El sistema analiza posibles cambios dentro de los cuales se encuentran la fecha y el medico.

 - El sistema recibe la informacion del usuario y modifica el turno guardado.

### Precondiciones

 - El usuario debe estar registrado y autenticado en el sistema.
 - El turno original debe estar confirmado y no debe estar dentro del período de cancelación.
 - El nuevo turno solicitado debe estar disponible.

### Postcondiciones

 - El turno original se actualiza con la nueva información.
 - Se envía una notificación al usuario confirmando el cambio de turno.
 - Se registra el cambio en el historial de turnos del usuario.






