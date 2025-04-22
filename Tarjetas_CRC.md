# Tarjetas CRC


### Tarjeta CRC:
 - Las Tarjetas CRC (Clase-Responsabilidad-Colaboración) constituyen una herramienta esencial en el enfoque de la programación orientada a objetos (POO). Se utilizan para identificar y definir las clases principales de un sistema, así como sus responsabilidades y colaboraciones dentro del contexto del sistema.


### Tarjeta CRC Paciente

- Nombre de la Clase: Paciente

- Superclase: Persona

- Subclase: -

- Pensamiento del objeto: Sé qué especialista requiero junto a mis datos personales. Necesito ver cuándo y con quién tengo turno. Avisare cuando no pueda asistir. Mis datos pueden cambiar. Quiero recordar mis turnos anteriores.

- Responsabilidades: Solicitar un turno, Consultar sus turnos programados, Cancelar un turno, Actualizar sus datos personales, Ver el historial de sus consultas.

- Colaboradores: Agenda, Turno, Médico,recepcionista.

- Propiedad: Nombre, apellido, fechaNacimiento, DNI, direccion,telefono,email.

[Paciente](https://drive.google.com/file/d/1dBI_MhTWrXPuv7pfWTipTFa4K3bT7Woq/view?usp=sharing)

### Tarjeta CRC Medico

- Nombre de la Clase: Médico

- Superclase: Persona

- Subclase: —

- Pensamiento del objeto: Quiero recordar turnos. Necesito ver mi agenda, registrar observaciones y diagnósticos. Puedo modificar turnos si es necesario. Quiero acceder al historial de consultas de mis pacientes.

- Responsabilidades: Visualizar y gestionar su agenda de turnos,Registrar diagnósticos y observaciones médicas,Acceder al historial clínico de sus pacientes,Modificar o cancelar turnos.

- Colaboradores: Turno,Paciente,HistoriaClinica,Agenda

- Propiedad a la que se referenciará:

- Nombre, Apellido, especialidad, matricula, Horarios de Atencion

[Medico](https://drive.google.com/file/d/1AuIMTf8kd3Op3kBHrJlsjSicwsYhGy0D/view?usp=sharing)


### Tarjeta CRC recepcionista

- Nombre de la Clase: Recepcionista

- Superclase: Persona

- Subclase: —

- Pensamiento del objeto: Me encargo de la gestión de la agenda. Registro nuevos pacientes.organizo turnos, cancelo citas si es necesario.Me encargo de asignar turnos.Me encargo de consultar o actualizar los datos de los pacientes.

- Responsabilidades: Registrar nuevos pacientes en el sistema,Asignar turnos a pacientes,Cancelar o reprogramar turnos,Consultar agenda de médicos,Consultar los datos o actualizar de un paciente.

- Colaboradores: Paciente ,Turno , Agenda, Médico , recepcionista

- Propiedad:Nombre , apellido, dni , email ,telefono , direccion

[Rcepcionista](https://drive.google.com/file/d/1bVrFrsV4KK9_MvGskRWXPKmcvkD1dNnq/view?usp=sharing)



### Tarjeta CRC turno

- Nombre de la Clase: Turno

- Superclase: —

- Subclase: —

- Pensamiento del objeto: Tengo una fecha y una hora asignada,se quien me va a atender , se a quien debo atender, mi estado puede cambiar segun la accion realizada.

- Responsabilidades: Conocer su fecha y hora, Conocer el paciente asignado, Conocer el médico asignado, Cambiar su estado.

- Colaboradores: Paciente, Médico,Recepcionista.

- Propiedad: fecha, hora, estado, paciente,motivo de cancelacion.

[Turno](https://drive.google.com/file/d/1e1W_-2se2xHq4II7pJSPXqRBKJejI8Yu/view?usp=sharing)



### Tarjeta CRC agenda

- Nombre de la Clase: Agenda

- Superclase: —

- Subclase: —

- Pensamiento del objeto: Organizo los turnos de un médico. Permito visualizar disponibilidad y asignar turnos nuevos.Muestro qué días y horarios están disponibles.Me encargo de mantener actualizada la disponibilidad para nuevos turnos,Asigno los turnos a los pacientes.

- Responsabilidades principales: Organizar agenda,Mostrar disponibilidad del médico,modificar o eliminar turnos,Filtrar por día o paciente,Asignar turno

- Colaboradores: Médico, Turno, Paciente

- Propiedad: fecha Inicio , fecha Fin, medicoId, listaTurnos,turno.

[Agenda](https://drive.google.com/file/d/1Xq2qaQsecmaGKN8qrjFQW2WlQQ17b_vo/view?usp=sharing)











  

