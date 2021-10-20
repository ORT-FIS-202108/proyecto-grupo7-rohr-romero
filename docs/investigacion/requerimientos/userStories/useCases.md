# User Stories y Use Cases

## User Story #1 - Iniciar sesión

### Narrativa
- **Como:** Usuario de la aplicación
- **Quiero:** Ingresar a mi cuenta
- **Para:** Poder ingresar mis gastos y controlar finanzas.

### Criterios de aceptación:
- Es responsivo y me dirige correctamente al sitio
- Ingreso a la aplicación y veo la pantalla de login con los campos usuario y contraseña para ingresar a la aplicación. 
- En la pantalla de login veo el botón "Iniciar sesión"
- En la pantalla de login veo el botón "Ingresar como invitado".
- El sistema valida que el usuario y contraseña estén correctos.


## Use Case #1 - Iniciar sesión

**Actor:** usuario
#### Curso normal para narrativa:

| **Acción de los actores**        | **Respuesta del sistema**           |
| ------------- |:-------------:|
| Ingresa a la aplicación y puede ver la página de iniciar sesión.       | Muestra la página de inicio |
| Ingresa con sus credenciales a su cuenta      | Muestra la página principal del sistema      |

### Cursos alternativos:

- Si el usuario ingresa mal las credenciales, se le niega el acceso y se le notifica que las credenciales son incorrectas.




## User Story #2 - Ingresar sesión como invitado

### Narrativa
- **Como:** Potencial usuario de la aplicación
- **Quiero:** Ingresar el sitio como invitado
- **Para:** poder explorar la aplicación y ver si me es útil utilizarla.

### Criterios de aceptación:
- Es responsivo y me dirige correctamente al sitio
- Presiono "Ingresar como invitado" y me redirige al sitio correctamente.
- Si ingreso datos, el sistema me dice que mi usuario no está registrado.

## Use Case #2 - Iniciar sesión como invitado

**Actor:** usuario
#### Curso normal para narrativa:

| **Acción de los actores**        | **Respuesta del sistema**           |
| ------------- |:-------------:|
| Ingresa a la aplicación y puede ver la página de iniciar sesión.        | Muestra la página de inicio |
| Selecciona la opción de “Ingresar como invitado”      | Muestra página principal     |
| Cualquier lugar que se desee ir del sitio      | Se muestran todos los campos y tablas vacías     |

### Cursos alternativos:

- No aplica ya que el usuario va a ingresar como invitado y no tiene que ingresar datos.
- Si ingresa datos y no está registrado, el sistema le notificará que las credenciales no son válidas.







## User Story #3 - Mis perfil de usuario

### Narrativa
- **Como:** Usuario de la aplicación
- **Quiero:** Poder mi perfil de usuario (mis datos personales)
- **Para:** Para editar algún dato o ir a mi cuenta bancaria

### Criterios de aceptación:
- Veo los datos personales y el balance de mi cuenta bancaria (previamente ingresada)
- Al presionar en el ícono de editar en un campo, el sistema habilita el campo para que el usuario edite.
- Puedo editar mis datos personales como nombre, apellido, teléfono, email, cuenta bancaria y el saldo de la misma.
- Guardo los campos editados y el sistema notifica al usuario vía email.
- Presiono click en la cuenta bancaria y me redirecciona a las páginas de bancos correctamente (según el banco correspondiente)

**Nota:** 
Se mostrarán disponibles los bancos: _ITAÚ, BBVA, BROU, SANTANDER, SCOTIABANK, HSBC_

## Use Case #3 - Mi Perfil de usuario

**Actor:** usuario
#### Curso normal para narrativa:

| **Acción de los actores**        | **Respuesta del sistema**           |
| ------------- |:-------------:|
| Selecciona la opción de la página principal “Mi perfil”         | Dirige a la sección “Mi perfil”  |
| Veo mis datos personales      | Veo toda la información con mis datos personales. Veo íconos para editar los campos.    |
| Presiono los íconos para editar y puedo editar los datos personales.      | Se guardan correctamente y se notifica al usuario.     |
| Se configuran notificaciones     | Se ejecuta la notificación correctamente     |

### Cursos alternativos:

- Si el usuario no tiene una cuenta y desea operar, se le pedirá que cree una cuenta




## User Story #4 - Panel de control

### Narrativa
- **Como:** Usuario de la aplicación
- **Quiero:** Poder registrar mis gastos mensuales 
- **Para:** Visualizar mejor el destino de mis fondos y poder planificar mejor mis finanzas.

### Criterios de aceptación:
- Veo el Saldo de mi cuenta para saber mi dinero restante (ingresos - gastos)
- Veo una gráfica con todos los gastos en porcentaje por tipo de gastos.
- Presiono el botón "añadir un gasto" y el sistema me despliega un popUp para ingresar los datos.
- Presiono el botón "definir presupuestos" y el sistema me redirecciona a la "USER STORY  #4.2".
- Veo un historial de los últimos gastos del mes.
- _Se asume como criterio de aceptación para todos los use cases que el sitio sea responsivo_




## Use Case #4 - Panel de control

**Actor:** usuario
#### Curso normal para narrativa:

| **Acción de los actores**        | **Respuesta del sistema**           |
| ------------- |:-------------:|
| Selecciona la opción de la página principal “Panel de control”         | Dirige a la sección “Panel de control” |
| Se ingresa el monto del gasto mensual      | Guarda correctamente los datos y actualiza la gráfica de gastos.    |
| Veo la gráfica con los gastos registrados     | El sistema me muestra todos los gastos en una gráfica.    |
| Veo el historial de los gastos registrados     | Veo una tabla con los últimos gastos del mes   |

### Cursos alternativos:

- Si el usuario no ingresa datos y oprime un botón para realizar una acción saltará una excepción.
- Si el usuario no tiene una cuenta y desea operar, se le pedirá crearse una

**Nota:** Para ingresar un gasto, se debe indicar la fecha actual y guardar todos los datos ingresados para el mes correspondiente. De esta manera se logra hacer un “tracking” organizado de las finanzas personales del cliente.





## User Story #5.1 - Añadir deuda

### Narrativa
- **Como:** Usuario de la aplicación
- **Quiero:** Poder Ingresar mis deudas
- **Para:** Visualizar mejor cuánto debo y tengo disponible para el mes.

### Criterios de aceptación:
- Veo una tabla con las deudas que tengo y sus cuotas.
- Veo una gráfica con las deudas y cuánto tengo pagado.
- Presiono ingresar una deuda y el sistema me despliega un PopUp para ingresar los datos.
- En la deuda puedo ingresar los plazos, ingresar las cuotas y marcar qué prioridad tiene.



## Use Case #5.1 - Añadir deuda

**Actor:** usuario
#### Curso normal para narrativa:

| **Acción de los actores**        | **Respuesta del sistema**           |
| ------------- |:-------------:|
| Selecciona la opción de la página principal “Panel de control”         | Dirige a la sección “Panel de control” |
| Se selecciona el botón “Añadir deuda”     | La página redirige a la sección “Nueva deuda” dentro de “Panel de control”    |
| Se ingresa el monto, cuota a pagar por mes, plazo de pago y prioridad    | Guarda correctamente los datos y los despliega en la tabla “Deudas pendientes”    |

### Cursos alternativos:

- Si se oprime “Añadir deuda” y hay campos vacíos, saltará una excepción.
- Si el usuario no tiene una cuenta y desea operar, se le pedirá crearse una



## User Story #5.2 - Definir presupuestos

### Narrativa
- **Como:** Usuario de la aplicación
- **Quiero:** Poder definir un presupuesto
- **Para:** Organizarme mejor y ver habilidad de pago para no excederme de mi presupuesto.

### Criterios de aceptación:
- Veo una gráfica con el total de mi presupuesto y cuánto llevo gastado.
- Veo las deudas según la prioridad definida.
- Presiono el ícono de editar en "Mis gastos fijos" y el sistema me permite ingresar asignar el monto de dinero que deseo destinar para pagar los determinados gastos recurrentes.
- Veo mis gastos imprescindibles y los prescindibles.
- Puedo editar mis ingresos.




## Use Case #5.2 - Definir presupuestos

**Actor:** usuario
#### Curso normal para narrativa:

| **Acción de los actores**        | **Respuesta del sistema**           |
| ------------- |:-------------:|
| Selecciona la opción de la página principal “Panel de control” y luego selecciona “Definir presupuestos”        | Dirige a la sección “Definir presupuestos” |
| Se selecciona/an la/ las deuda/as a saldar  y se destinan los fondos necesarios     | Guarda correctamente los datos y despliega en otra tabla “Plan de saldo de deudas”    |
| Se define qué cantidad de dinero se desea gastar por cada área. Ej: en “Gastos de casa” $18.000 , en “Gastos fijos” $25.000 , etc.    | Se guardan correctamente los datos    |

### Cursos alternativos:

- Si el usuario también desea asignar más dinero del que tiene, saltará una excepción
- Si no tiene deudas, fin del caso 2 (fila 2)
- Si el usuario no tiene una cuenta y desea operar, se le pedirá crearse una











Narrativa:
Como: Usuario de la aplicación
Quiero: Poder definir un presupuesto
Para: Organizarme mejor y ver habilidad de pago para no excederme de mi presupuesto.

Criterios de aceptación:
Veo una gráfica con el total de mi presupuesto y cuánto llevo gastado.
Veo las deudas según la prioridad definida.
Presiono el ícono de editar en "Mis gastos fijos" y el sistema me permite ingresar asignar el monto de dinero que deseo destinar para pagar los determinados gastos recurrentes.
Veo mis gastos imprescindibles y los prescindibles.
Puedo editar mis ingresos.


Use Case #5.2 - Definir presupuestos
Actor: usuario
Curso normal:

Acción de los actores
Respuesta del sistema


Selecciona la opción de la página principal “Panel de control” y luego selecciona “Definir presupuestos”
Dirige a la sección “Definir presupuestos”
Se selecciona/an la/ las deuda/as a saldar  y se destinan los fondos necesarios
Guarda correctamente los datos y despliega en otra tabla “Plan de saldo de deudas”
Se define qué cantidad de dinero se desea gastar por cada área. Ej: en “Gastos de casa” $18.000 , en “Gastos fijos” $25.000 , etc.
Se guardan correctamente los datos 



### Cursos alternativos:

Si el usuario también desea asignar más dinero del que tiene, saltará una excepción
Si no tiene deudas, fin del caso 2 (fila 2)
Si el usuario no tiene una cuenta y desea operar, se le pedirá crearse una

