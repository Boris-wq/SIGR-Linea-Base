
# Documentación funcional de los módulos del SIGR

## 1. Introducción

El Sistema Integral de Gestión de Restaurante estará dividido en cinco módulos. Cada uno tendrá una función dentro de la operación del negocio y trabajará de manera relacionada con los demás.

En este documento se explica qué hará cada módulo, quién podrá utilizarlo y qué información manejará.

## 2. Módulo de autenticación de usuarios

### Descripción

Este módulo será la puerta de entrada al sistema. Su función será identificar a las personas que ingresen y permitirles acceder únicamente a las opciones correspondientes a su perfil.

### Usuarios

- Cliente.
- Mesero.
- Administrador.

### Funciones principales

- Registrar o crear cuentas de usuario según las condiciones del restaurante.
- Permitir el inicio y cierre de sesión.
- Validar las credenciales ingresadas.
- Reconocer el rol de cada persona.
- Restringir el acceso a las funciones administrativas.

### Información que manejará

Nombre del usuario, correo electrónico, contraseña protegida, rol asignado y estado de la cuenta.

### Resultado esperado

Cada persona podrá ingresar al sistema y utilizar las opciones que correspondan a sus responsabilidades.

## 3. Módulo de menú digital

### Descripción

Este módulo permitirá mostrar los productos que ofrece el restaurante. También facilitará la actualización de la información cuando se agreguen nuevos platos o cambien los precios.

### Usuarios

- Cliente.
- Mesero.
- Administrador.

### Funciones principales

- Consultar los platos disponibles.
- Organizar los productos por categorías.
- Registrar nuevos platos.
- Modificar nombres, descripciones y precios.
- Cambiar la disponibilidad de un producto.
- Retirar temporalmente de la oferta los platos que no se encuentren disponibles.

### Información que manejará

Nombre del plato, descripción, categoría, precio, disponibilidad e imagen cuando se encuentre habilitada.

### Resultado esperado

Los clientes y meseros podrán consultar un menú actualizado. El administrador podrá mantener organizada la oferta gastronómica.

## 4. Módulo de registro y seguimiento de pedidos

### Descripción

Este módulo permitirá registrar los pedidos realizados por los clientes y consultar su avance. La información quedará organizada para facilitar la atención y evitar confusiones durante la preparación.

### Usuarios

- Cliente.
- Mesero.
- Administrador.

### Funciones principales

- Crear un nuevo pedido.
- Agregar platos y cantidades.
- Calcular el valor de los productos seleccionados.
- Consultar los pedidos registrados.
- Actualizar el estado de cada pedido.
- Identificar si el servicio corresponde a mesa, recogida o domicilio.

### Estados del pedido

El proceso podrá manejar los siguientes estados:

1. Registrado.
2. Confirmado.
3. En preparación.
4. Listo.
5. En entrega, cuando sea a domicilio.
6. Entregado.
7. Cancelado.

### Información que manejará

Número del pedido, fecha, productos solicitados, cantidades, valor total, tipo de servicio y estado actual.

### Resultado esperado

El personal podrá conocer qué pedidos están pendientes y cuáles ya fueron preparados o entregados.

Cuando se trate de un domicilio, se podrá consultar el avance de la entrega. El rastreo GPS no se incluye en esta primera definición.

## 5. Módulo de reservas por fecha y hora

### Descripción

Este módulo ayudará a organizar las solicitudes de reserva. Permitirá conocer qué clientes desean ocupar una mesa y en qué momento.

### Usuarios

- Cliente.
- Mesero.
- Administrador.

### Funciones principales

- Registrar solicitudes de reserva.
- Seleccionar fecha y hora.
- Indicar el número de personas.
- Consultar la disponibilidad de mesas.
- Confirmar o cancelar reservas.
- Consultar las reservas pendientes.

### Información que manejará

Nombre del cliente, datos de contacto, fecha, hora, cantidad de personas y estado de la reserva.

### Estados de la reserva

- Solicitada.
- Confirmada.
- Atendida.
- Cancelada.
- No asistió.

### Resultado esperado

El restaurante podrá organizar mejor la atención y reducir los inconvenientes relacionados con la disponibilidad de mesas.

## 6. Módulo de cierre de caja y reportes de ventas

### Descripción

Este módulo estará enfocado en el control de los ingresos del restaurante. Su finalidad será reunir la información de los pagos y facilitar la revisión de las ventas realizadas durante el día.

### Usuarios

- Administrador.
- Mesero, de acuerdo con los permisos asignados.

### Funciones principales

- Consultar los pedidos pagados.
- Registrar los pagos relacionados con cada pedido.
- Identificar los medios de pago utilizados.
- Consultar el total de las ventas.
- Realizar el cierre diario de caja.
- Generar reportes de ventas.

### Información que manejará

Número del pedido, valor pagado, medio de pago, fecha de la operación, responsable y total de ventas.

### Resultado esperado

El administrador podrá revisar los ingresos del restaurante y consultar un resumen de las operaciones realizadas durante la jornada.

## 7. Relación entre los módulos

Los módulos no funcionarán de manera aislada. Cada uno aportará información para el funcionamiento general del restaurante.

La autenticación controla el ingreso de los usuarios. El menú presenta los productos disponibles y el módulo de pedidos registra las solicitudes. Las reservas organizan la atención de las mesas. Finalmente, caja reúne la información de los pagos y permite revisar las ventas.

Esta relación permitirá mantener una operación más organizada y facilitar el seguimiento de la información.

## 8. Consideraciones para la línea base

La descripción de estos cinco módulos formará parte de la línea base documental del SIGR.

Si posteriormente se modifica alguna función, será necesario revisar el documento y registrar el cambio en el repositorio de GitHub. De esta manera se conservará el historial y se podrá identificar qué versión fue aprobada.
