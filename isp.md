# Principio de Segregacion de Interfaces (ISP)

 - El Principio de Segregación de Interfaces (ISP) se refiere a la idea de que una clase no debe estar obligada a implementar interfaces que no utiliza. Es decir, si una clase implementa una interfaz, solo debe hacerlo para los métodos que realmente necesita. Si una interfaz tiene métodos que una clase no va a usar, es mejor dividir esa interfaz en varias más pequeñas y específicas.
   - El tipo del principio SOLID al que pertenece el ISP es un principio de diseño de interfaces. Ayuda a estructurar interfaces que sean lo más específicas posible, evitando que las clases implementen métodos que no les interesan.


- El problema que aborda el ISP se da en situaciones donde las interfaces son demasiado grandes o genéricas, forzando a las clases que las implementan a incluir métodos innecesarios. Esto puede hacer que:

  - Las clases implementen métodos que nunca usan.

  - Se incremente el acoplamiento entre clases que no deberían estar relacionadas.

  - El código se vuelva más difícil de mantener porque los cambios en una interfaz pueden afectar a múltiples clases que no deberían verse afectadas.
 
  - Se introduzca código muerto (código que nunca se ejecuta o que tiene sentido solo en casos limitados), lo que puede hacer más difícil la evolución del sistema.

  ### Motivacion

  - El problema surge cuando las interfaces son demasiado generales y no están bien distribuidas entre las clases. Este enfoque puede resultar en falta de flexibilidad y dificultar la extensibilidad del sistema. Si el sistema crece o se requieren cambios en una clase, es probable que otras clases se vean afectadas debido a la implementación de métodos innecesarios, lo que puede generar errores o redundancias.

  ### Ejemplo

   - Un ejemplo pdrian ser los estudiantes en la sociedad, se dividen en especialidades para en un futuro cumplir un rol.
     

     

