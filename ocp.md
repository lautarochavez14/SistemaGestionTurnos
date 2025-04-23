# Principio de Abierto/Cerrado (OCP)

-El propósito central del Principio de Abierto/Cerrado es permitir que el software pueda ampliarse con nuevas funciones sin tener que alterar el código que ya existe. En el sistema utilizado para administrar los turnos médicos, la parte encargada de enviar notificaciones estaba construida de forma inflexible. Toda la lógica relacionada con el envío de correos electrónicos, mensajes de texto o llamadas telefónicas se encontraba en una única estructura. Cada vez que era necesario incorporar un nuevo medio de notificación (como WhatsApp o alertas en dispositivos móviles), se debía modificar directamente ese código, lo que provocaba errores, afectaba funcionalidades previas y dificultaba el mantenimiento general del sistema.

El principio OCP sugiere que un sistema debe estar disponible para ser ampliado, pero sin necesidad de modificar lo ya implementado. En otras palabras, debería ser posible incorporar nuevas funcionalidades (como un canal adicional de notificación) sin cambiar el código que ya está en funcionamiento. Para alcanzar esto, se reorganizó la lógica del sistema en módulos independientes, asignando a cada tipo de notificación su propio componente. De este modo, si se desea sumar un nuevo canal de aviso, se hace a través de una extensión, sin interferir con lo que ya está implementado. Esto hace que el sistema sea más adaptable, confiable y fácil de mantener ante futuros cambios.

## Motivacion 

- En el sistema de gestión de turnos médicos, aparecían complicaciones cada vez que se intentaban agregar nuevas funcionalidades, como diferentes tipos de notificaciones dirigidas a pacientes y profesionales de la salud. Inicialmente, solo se utilizaba el correo electrónico, pero con el tiempo se quiso incorporar el envío de SMS entre otros.

El problema era que al añadir un nuevo canal de comunicación, era necesario modificar el código existente. Esto podía afectar funcionalidades que ya estaban operando correctamente, dificultar las pruebas del sistema y volverlo más complejo.

El principio de abierto/cerrado (OCP) sugiere que los sistemas deben diseñarse de forma que se puedan extender sin necesidad de alterar el código que ya está funcionando. Es decir, permitir incorporar nuevas características sin modificar las ya existentes.

### Ejemplo 

- En tu casa, tienes enchufes en la pared. Cuando compras un nuevo electrodoméstico no necesitas cambiar los enchufes. Solo conectas el nuevo aparato, caso contrario tendrias que romper la pared para agregar un nuevo electrodomestivo.

Eso es aplicar el Principio de Abierto/Cerrado:

Los enchufes no se modifican (cerrados a cambios).

## Estructura de clase

Puedes agregar nuevos aparatos fácilmente (abiertos a extensión).

![OCP](https://github.com/user-attachments/assets/17b1197c-22a5-4f18-becf-f7d6732bc5f2)

[Estructura de clases](https://drive.google.com/file/d/1ouQ0WHXVj23v6lTY2etp5T7seG8u7Lgl/view?usp=sharing)




