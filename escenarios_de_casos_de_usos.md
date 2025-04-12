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


![caso 2](https://github.com/user-attachments/assets/db5c9736-9ced-4335-9463-9921047bded6)


## Caso 3: Cancelar turno

### Descripcion general

 - Permite al usuario cancelar un turno ya pedido.
 
### Flujo de eventos 

 - El usuario ingresa al sistema.

 - El usuario se dirige a "Cancelar turno".

 - El usuario cancela el turno previamente pedido.

### Precondiciones

 - El usuario debe estar registrado y autenticado en el sistema.
 - El turno debe estar confirmado y dentro del período de cancelación permitido.


### Postcondiciones

 - El turno se marca como cancelado en el sistema.
 - Se envía una notificación al usuario confirmando la cancelación.
 - Se actualiza la disponibilidad del turno en el sistema.
   
![caso 3](https://github.com/user-attachments/assets/a0a062e8-7dcc-4da7-8ba9-25b98198cd0f)

## Caso 4: Pedir turno

### Descripcion general

 - Permite al usuario pedir un turno.

### Flujo principal de eventos

 - El usuario ingresa al sistema.

 - El usuario selecciona la fecha y medico para su turno.

 - El usuario solicita el turno.

 - El sistema agenda el turno.

### Precondiciones

 - El usuario debe estar autenticado y tener un método de pago válido.

### Postcondiciones:

 - La compra se ha completado y el usuario recibe la confirmación.


![caso 4](https://github.com/user-attachments/assets/7e043e9d-d8f1-46ff-a5c2-b7d10df82891)


## Caso 5: Consulta de turnos

### Descripcion general

 - Permite al usuario visualizar los turnos solicitadoss.

### Flujo principal de eventos

  - El usuario ingresa al sistema.

  - El usuario se dirige a "Consultar turnos".

  - El sistema muestra el historial de turnos del usuario.

### Precondiciones

 - El usuario debe estar registrado y autenticado en el sistema.

### Postcondiciones

 - El sistema muestra una lista de los turnos programados del usuario.
 - Se registra la consulta en el historial de actividades del usuario.


![Captura de pantalla (23)](https://github.com/user-attachments/assets/6d49f5ba-2190-4678-a663-b52b2cd81023)




 
