# Tarjetas CRC


### Tarjeta CRC:
 - Las Tarjetas CRC (Clase-Responsabilidad-Colaboración) constituyen una herramienta esencial en el enfoque de la programación orientada a objetos (POO). Se utilizan para identificar y definir las clases principales de un sistema, así como sus responsabilidades y colaboraciones dentro del contexto del sistema.


### CRC Caso1: Notificacion

- Nombre de la clase: Notificacion

- Superclase: Sistema

- Subclase:--

- Pensamiento del objeto: Tengo la fecha, hora, paciente y medico especialista para armar la notificacion que sera enviada al usuario paciente.

- Responsabilidades: Conocer la fecha y hora del turno, los datos del usuario y correo.

- Colaboradores: Solicitud de turno

- Propiedades: Fecha, hora, idusuario, medico.

  ![crc 1](https://github.com/user-attachments/assets/f180b7dc-0665-438b-a16f-443f7a6904e5)


### CRC Caso2: Cambio de turno

- Nombre de la clase: Cambio de turno

- Superclase: Sistema

- Subclase: --

- Pensamiento del objeto: Conocer los datos del turno, posibles cambios y datos del usuario.

- Responsabilidades: Reconocer fecha y hora del turno a cambiar.

- Colaboradores: Solicitud de turno, notificacion

- Propiedades: Fecha, hora, idusuario, especialidad medico


![crc2](https://github.com/user-attachments/assets/702596bf-fbe1-474d-97c2-8678e5aea9cf)


### CRC Caso3: Cancelar turno

- Nombre de la clase: Cancelar turno

- Superclase: Sistema

- Subclase: Gestion de turno

- Pensamiento del objeto: conocer los datos del turno a cancelar, y notificar la cancelacion del mismo

- Responsabilidades: Cancelar el turno ya pedido y marcarlo como cancelado en la agenda

- Colaboradores: Solicitar turno, notificacion

- Propiedades: turno, usuario, medico, agenda.


![crc 3](https://github.com/user-attachments/assets/57c23a50-00b0-430c-9d78-9df94ae34fe6)


### CRC Caso4: Pedir turno

- Nombre de la clase: pedir turno

- Superclase: Sistema

- Subclase:--

- Pensamiento del objeto: Debo registrar el turno solicitado con los datos especificos (fecha, hora, medico, especialidad e IDusuario.

- Responsabilidades: Plasmar el turno solicitado sobre la agenda del medico

- Colaborardores: Consulta de turnos, notificacion

- Propiedades: Medico, usuario, agenda


![crc 4](https://github.com/user-attachments/assets/d18040b5-f93a-4ec6-abef-4a735300dee6)


### CRC Caso5: Consulta de turnos

- Nombre de la clase: Consulta de turnos

- Superclase: Sistema

- Subclase:--

- Pensamiento del objeto: Debo mostrar la agenda sobre los turnos disponibles

- Responsabilidades: Mostrar al usuario los turnos disponibles con su especialidad y medico a cargo

- Colaboradores: pedir turno

- Propiedades: Usuario, medico, turno

  
![Captura de pantalla (28)](https://github.com/user-attachments/assets/651da0ed-0fa0-46fc-ac3e-db635bec0a8c)









  

