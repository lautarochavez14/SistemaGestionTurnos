# Principio de Sustitucion de Liskov (LSP)

 - Este principio está vinculado al uso de la herencia en diseño orientado a objetos. Su propósito es garantizar que las clases hijas puedan sustituir a sus clases base sin alterar el comportamiento correcto del sistema. En el sistema de gestión de turnos médicos, se creó una clase principal llamada Usuario, de la cual se derivaron clases específicas como Paciente, Médico y Recepcion.

- El inconveniente apareció cuando algunas de estas subclases modificaban métodos heredados de manera que rompían la lógica del sistema. Por ejemplo, en ciertos contextos se esperaba trabajar con un objeto del tipo Usuario, pero al utilizar un Administrador, el sistema fallaba porque esta subclase no implementaba adecuadamente funciones clave como la de reservar turnos. Esto iba en contra del principio, ya que todas las subclases de Usuario deberían poder emplearse de forma intercambiable sin que se altere el funcionamiento del sistema.

- Para evitar que el sistema fallara o se volviera inestable, se implementaban excepciones manuales, lo que aumentaba la complejidad y el riesgo de cometer errores.

El principio de sustitución de Liskov establece que una clase hija debe ser capaz de sustituir a su clase padre sin afectar el funcionamiento del sistema. En este caso, si un Administrador no puede realizar las mismas acciones que un Usuario (como solicitar turnos), se estaría violando este principio.

La solución consistió en redefinir de manera precisa qué acciones podía llevar a cabo cada tipo de usuario. De esta forma, cada uno se limitaba a sus propias funciones, lo que hizo el sistema más organizado, seguro y fácil de gestionar.

### Ejemplo

 - Como ejemplo tomaremos un auto y una bicicleta, los dos sirven para moverse pero sus caracteristicas son muy distintas.


## Estructura de clases

![lsp](https://github.com/user-attachments/assets/fa2a4ebb-36e0-45ea-a81f-5f34c12522d1)

[Estructura de clases](https://drive.google.com/file/d/1IQz6b4F52KNh8vOaMZjCxVGa4RseJS4s/view?usp=sharing)


   
