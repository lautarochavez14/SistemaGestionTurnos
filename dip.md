# Principio de Inversion de Dependencias (DIP)

- En la plataforma para la administración de turnos médicos, varios componentes esenciales estaban estrechamente ligados a servicios concretos, como una determinada base de datos o un sistema específico para el envío de correos electrónicos. Esto provocaba que cualquier cambio en dichos servicios afectara al sistema en su totalidad, generando fallos y dificultando la incorporación de nuevas tecnologías o procesos de migración. El enfoque propuesto plantea modificar esta estructura para que la lógica central del sistema no dependa directamente de implementaciones particulares. En su lugar, se recurre a capas de abstracción (por ejemplo, un "módulo de notificaciones" en lugar de un "servicio de correo electrónico"). Así, se pueden realizar cambios o reemplazos en los servicios sin interferir con el funcionamiento general, lo que mejora la flexibilidad, la reutilización y la capacidad del sistema para evolucionar con el tiempo.


## Motivacion 

 - En la solución destinada a gestionar los turnos médicos, uno de los principales inconvenientes era que los módulos de nivel superior —como la lógica encargada de organizar citas y asignar profesionales— estaban estrechamente conectados a componentes de nivel inferior, tales como bases de datos específicas o mecanismos concretos de notificación, como el correo electrónico. Esta dependencia directa provocaba que cualquier ajuste en esos elementos técnicos afectara el funcionamiento global del sistema.

Para resolver este problema, se implementó el principio de inversión de dependencias (DIP), reorganizando la arquitectura para que la lógica central pasara a depender de abstracciones como interfaces para servicios de notificación, acceso a datos, entre otros; en lugar de depender directamente de soluciones particulares. Por ejemplo, en vez de vincular el sistema de turnos a un servicio de correo específico, se definió una interfaz genérica llamada “Servicio de Notificación”, con la cual interactúa el sistema sin necesidad de conocer cómo se implementa por detrás. Esto facilitó la posibilidad de modificar o sustituir el sistema de notificación sin impactar el resto de la aplicación. De esta manera, el código principal quedó desacoplado de los detalles técnicos, volviendo la solución más adaptable, sencilla de probar y más fácil de mantener con el paso del tiempo.

### Ejemplo 

- Antes, muchos teléfonos venían con una entrada de auriculares específica. Si cambiabas de marca, tus auriculares ya no servían.

 Ahora, gracias a tecnologías como Bluetooth (una abstracción), puedes usar los mismos auriculares inalámbricos con cualquier celular, sin importar la marca.
