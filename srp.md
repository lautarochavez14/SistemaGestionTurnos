# Principio de responsabilidad unica(SRP)

- El Principio de Responsabilidad Única (Single Responsibility Principle, SRP) busca garantizar que una clase tenga únicamente un motivo para modificarse. En otras palabras, cada clase debe cumplir con una sola función específica, y todas sus operaciones deben estar alineadas con esa función.

En el contexto de un sistema para organizar citas médicas, se detectaron módulos que combinaban múltiples tareas dentro de una sola estructura. Por ejemplo, una parte del sistema era responsable, al mismo tiempo, de agendar citas, verificar la disponibilidad del profesional, enviar avisos al paciente y almacenar la información en la base de datos. Este principio sugiere dividir esas actividades en unidades separadas, de forma que cada una se especialice en una función particular: una se dedica a programar las citas, otra a confirmar la disponibilidad, otra a gestionar los avisos, y otra a registrar los datos.

## Motivacion 

### Ejemplo

- Imagina una empresa que realiza envíos de paquetes, y tiene una aplicación para gestionar las entregas. En esta aplicación hay una sola clase llamada GestorEnvios, y hace de todo:

   - Crea el pedido de envío.

   - Calcula el costo del envío según distancia y peso.

   - Genera la etiqueta del paquete.

   - Contacta al repartidor.

   - Notifica al cliente con el estado del pedido.

   - Almacena los datos del envío en la base de datos.
  

- Al tener múltiples funciones dentro de una sola clase:

   - Cada vez que se modifica la forma de calcular el costo, hay que revisar toda la clase.

   - Si se actualiza el formato de las notificaciones, se corre el riesgo de romper la lógica de asignación de repartidores.

   - Se vuelve difícil probar partes del sistema por separado.

   - El código se vuelve frágil y difícil de escalar si en el futuro se quiere cambiar el sistema de mensajería, por ejemplo.


### El Principio de Responsabilidad Única sugiere dividir responsabilidades en clases diferentes:

PedidoEnvioCreator → se encarga de crear el pedido.

CalculadoraCostos → se especializa en calcular el precio del envío.

EtiquetaGenerador → genera etiquetas.

AsignadorRepartidores → gestiona quién entrega.

NotificadorCliente → envía mensajes al cliente.

BaseDatosEnvios → guarda la información.

Cada clase tiene una sola razón para cambiar, lo que hace el sistema:

Modular y fácil de mantener.

Más seguro ante errores por cambios.

Reutilizable (por ejemplo, la clase que calcula costos puede usarse en otro servicio).

# Estructura de clases

![estructuraclase](https://github.com/user-attachments/assets/b94641a1-25e5-43f8-b268-269bffee7f73)

[Estructura de clases](https://drive.google.com/file/d/1oQXrOuHMdi9tpImqi_DxNHRIcTrxfBV_/view?usp=sharing)






