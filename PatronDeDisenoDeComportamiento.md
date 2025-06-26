## Patrón de Diseño de Comportamiento: Observer
- Proposito y Tipo del Patron
- Tipo: Comportamiento
- Proposito:
El patrón Observer permite definir una relación de dependencia uno-a-muchos entre objetos, de manera que cuando uno cambia de estado, todos sus dependientes son notificados y actualizados automáticamente.

Por ejemplo:
El patron Observer se utiliza para notificar a los sistemas de turnos cuando un paciente realiza una acción que los involucra, como solicitar o cancelar un turno. De este modo, se mantiene actualizada la agenda del profesional médico y se avisa a otros sistemas como el de mensajeria.

### Motivacion
En el sistema de turnos médicos, surgió la necesidad de automatizar las notificaciones a múltiples componentes del sistema cuando un paciente crea, reprograma o cancela un turno.

- Problema:
El sistema enviaba manualmente actualizaciones a cada componente (agenda del médico, historial del paciente, sistema de mensajería), lo que aumentaba la complejidad y el riesgo de errores.

- Solucion con Observer:
El patrón Observer permite que cada componente del sistema se registre como "observador" del módulo de turnos. Cuando un turno es modificado, se notifica automáticamente a todos los observadores registrados, sin acoplar directamente el módulo de turnos a cada componente.

### Estructura de Clases (Diagrama UML)
