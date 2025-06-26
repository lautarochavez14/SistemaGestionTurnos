### Patrón de Diseño Creacional: Singleton

 - Propósito y Tipo del Patrón
  - Tipo: Creacional
  - Propósito:
- El patrón Singleton se utiliza para restringir la creación de múltiples instancias de una clase, asegurando que sólo exista una única instancia globalmente accesible.
Por ejemplo:
"El patrón Singleton se utiliza para garantizar que un sistema de configuración tenga una única instancia compartida por toda la aplicación, evitando inconsistencias y redundancia de información."

### Motivación
- En muchos sistemas, como aplicaciones de gestión de pacientes en un hospital, es importante que ciertos recursos como la configuración del sistema, las estadísticas o la conexión a una base de datos estén centralizados.
Permitir múltiples instancias podría generar conflictos o duplicación de recursos, como múltiples accesos simultáneos a una base de datos con distintos estados.

 - Problema:
Un sistema de turnos médicos manejado manualmente por un recepcionista causaba filas largas y errores al registrar pacientes en varias listas al mismo tiempo.

- Solución con Singleton:
La aplicación de este patrón permite crear un sistema centralizado de acceso a los datos del paciente. Solo se crea una única instancia del gestor de pacientes, garantizando integridad y sincronización.
La clase PacienteManager ahora se asegura de que solo haya una única instancia compartida en toda la aplicación.

### Estructura de Clases
