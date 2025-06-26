 ## Patrón de Diseño Estructural: Adapter
-  Propósito y Tipo del Patrón
- Tipo: Estructural
- Propósito:
 El patrón Adapter permite que clases con interfaces incompatibles trabajen juntas.
Por ejemplo:
"El patrón Adapter se utiliza para conectar el sistema de gestión de turnos con un servicio externo de mensajería que tiene una interfaz distinta, permitiendo que los mensajes de confirmación se envíen automáticamente a los pacientes."

### Motivación
En el desarrollo de un sistema de turnos médicos, se decidió integrar una API externa para enviar notificaciones por WhatsApp. Sin embargo, esta API tenía una interfaz completamente distinta a la que ya usaban las clases del sistema interno para enviar correos electrónicos.

 - Problema:
El sistema interno esperaba una interfaz Notificador con un método enviarMensaje(destinatario, contenido), mientras que la API externa usaba un método diferente como sendTo(phone, text).

 - Solución con Adapter:
Se implementó el patrón Adapter para crear una clase intermedia que tradujera la interfaz externa a la esperada por el sistema. Así, se logró integrar la nueva funcionalidad sin modificar el código existente, promoviendo la reutilización y separación de responsabilidades.

### Estructura de Clases (Diagrama UML)
