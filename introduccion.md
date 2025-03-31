
- [Introduccion](#introduccion)
- [Fundamentos](#Fundamentos)
- [Requisitos iniciales](#Requisitos)
- [Casos de uso](#casos)
- [Boceto inicial](#Boceto)

# Introducción(#Introduccion)


¿Qué es la Programación Orientada a Objetos (POO)?
La Programación Orientada a Objetos (POO) es un paradigma de programación basado en la organización del código en objetos, que representan entidades del mundo real.
Es importante porque permite crear software modular, reutilizable y fácil de mantener.

# Fundamentos de POO (#Fundamentos)

### Abstracción
Es la capacidad de representar elementos del mundo real en el código.
Ejemplo: Un "Auto" puede representarse con atributos (marca, modelo) y métodos (arrancar, frenar).

### Encapsulamiento
Protege los datos de un objeto, permitiendo acceso solo a través de métodos específicos.
Ejemplo: Un "Cajero Automático" no permite acceso directo al dinero, solo mediante transacciones.

### Herencia
Permite que una clase reutilice características de otra.
Ejemplo: Un "Auto Deportivo" hereda de la clase "Auto", pero añade características como mayor velocidad.

### Polimorfismo
Permite que una misma acción tenga diferentes comportamientos según el objeto.
Ejemplo: Un "Animal" puede hacer un sonido, pero cada tipo de animal emite un sonido diferente (perro: ladrido, gato: maullido).


# Requisitos iniciales del sistema (#Requisitos)
- Registro de usuarios: El sistema debe permitir la creación y gestión de usuarios.

- Gestión de turnos: Los usuarios deben poder solicitar, cancelar y reprogramar turnos.

- Notificaciones: El sistema debe enviar recordatorios de turnos vía correo o mensaje.

- Historial de turnos: Se debe permitir consultar turnos pasados.

- Control de acceso:Solo usuarios registrados pueden acceder a ciertas funciones.
# Casos de uso
 ## Caso 1
   ### Registro de usuario
 - Actores involucrados: Usuario y sistema
 - Descripción breve: Permite a un nuevo usuario crear una cuenta en la plataforma.
- Flujo principal de eventos
1. El usuario accede a la página de registro.
2. El usuario ingresa su información personal (nombre, correo, contraseña).
3. El sistema valida la información ingresada.
4. El sistema crea una nueva cuenta y envía un correo de confirmación.
5. El usuario recibe el correo y confirma su registro.
- Precondiciones: El usuario no debe tener una cuenta existente.
- Postcondiciones: El usuario tiene una cuenta activa en el sistema.

## Caso 2
  ### Inicio de Sesión
- Actores involucrados: Usuario, Sistema
- Descripción breve: Permite a un usuario registrado acceder a su cuenta.
- Flujo principal de eventos:
1. El usuario accede a la página de inicio de sesión.
2. El usuario ingresa su correo y contraseña.
3. El sistema valida las credenciales.
4. El sistema redirige al usuario a su panel de control.
- Precondiciones: El usuario debe tener una cuenta registrada.
- Postcondiciones: El usuario está autenticado y tiene acceso a su cuenta.

## Caso 3
  ### Recuperación de Contraseña
- Actores involucrados: Usuario, Sistema.
- Descripción breve: Permite a un usuario recuperar su contraseña en caso de olvido.
- Flujo principal de eventos:
1. El usuario accede a la opción de "Olvidé mi contraseña".
2. El usuario ingresa su correo electrónico.
3. El sistema envía un enlace de recuperación al correo proporcionado.
4. El usuario sigue el enlace y establece una nueva contraseña.
- Precondiciones: El usuario debe haber registrado su correo en la cuenta.
- Postcondiciones: El usuario ha restablecido su contraseña y puede iniciar sesión.

 ## Caso 4
  ### Pedir turno
- Nombre del caso de uso: Pedir turno
- Actores involucrados: Usuario, Sistema, Proveedor.
- Descripción breve: Permite a un usuario pedir un turno dentro de las especialidades.
- Flujo principal de eventos:
1. El usuario navega por el catálogo especialidades.
2. El usuario selecciona una especialidad.
3. El usuario procede al pago.
4. El sistema procesa el pago y confirma el turno.
5. El sistema envía un recibo al usuario.
- Precondiciones: El usuario debe estar autenticado y tener un método de pago válido.
- Postcondiciones: La compra se ha completado y el usuario recibe la confirmación.

## Caso 5
  ### Cierre de Sesión
- Actores involucrados: Usuario, Sistema.
- Descripción breve: Permite a un usuario cerrar su sesión en la plataforma.
- Flujo principal de eventos:
1. El usuario selecciona la opción de cerrar sesión.
2. El sistema finaliza la sesión del usuario.
3. El sistema redirige al usuario a la página de inicio.
- Precondiciones: El usuario debe estar autenticado.
- Postcondiciones: El usuario ha cerrado sesión y no tiene acceso a su cuenta hasta que inicie sesión nuevamente
  
# Boceto inicial del diseño de clases (#Boceto)ç

![](boceto inicial.drawio.html)

https://drive.google.com/file/d/1o6qPzOSaIVrl_R35Emcjz081xn35yq5y/view?usp=sharing

