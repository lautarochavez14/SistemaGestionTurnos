# Principio de responsabilidad unica(SRP)

- El Principio de Responsabilidad Única (Single Responsibility Principle, SRP) busca garantizar que una clase tenga únicamente un motivo para modificarse. En otras palabras, cada clase debe cumplir con una sola función específica, y todas sus operaciones deben estar alineadas con esa función.
 En el contexto de un sistema para organizar citas médicas, se detectaron módulos que combinaban múltiples tareas dentro de una sola estructura. Por ejemplo, una parte del sistema era responsable, al mismo tiempo, de agendar citas, verificar la disponibilidad del profesional, enviar avisos al paciente y almacenar la información en la base de datos. Este principio sugiere dividir esas actividades en unidades separadas, de forma que cada una se especialice en una función particular: una se dedica a programar las citas, otra a confirmar la disponibilidad, otra a gestionar los avisos, y otra a registrar los datos.

## Motivacion 

- Uno de los mayores inconvenientes en el sistema de administración de turnos médicos radicaba en que varios componentes debían cumplir con múltiples funciones simultáneamente. Por ejemplo, una misma parte del sistema se encargaba de agendar un turno, comprobar la disponibilidad del profesional, notificar al paciente y guardar toda esa información en la base de datos. Este modelo de "todo en uno" provocaba diversos inconvenientes: el código se volvía difícil de interpretar, cualquier modificación impactaba al sistema completo y los errores eran más complejos de detectar y solucionar.

### Ejemplo

- Imagina una empresa que realiza envíos de paquetes, y tiene una aplicación para gestionar las entregas. En esta aplicación hay una sola clase llamada GestorEnvios, y hace de todo:

- Al tener múltiples funciones dentro de una sola clase:

   - Cada vez que se modifica la forma de calcular el costo, hay que revisar toda la clase.

   - Si se actualiza el formato de las notificaciones, se corre el riesgo de romper la lógica de asignación de repartidores.

   - Se vuelve difícil probar partes del sistema por separado.

   - El código se vuelve frágil y difícil de escalar si en el futuro se quiere cambiar el sistema de mensajería, por ejemplo.

   - El Principio de Responsabilidad Única sugiere dividir responsabilidades en clases diferentes:


# Estructura de clases

![estructuraclase](https://github.com/user-attachments/assets/b94641a1-25e5-43f8-b268-269bffee7f73)

[Estructura de clases](https://drive.google.com/file/d/1oQXrOuHMdi9tpImqi_DxNHRIcTrxfBV_/view?usp=sharing)






