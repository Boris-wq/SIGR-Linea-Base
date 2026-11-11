
# Estructura de datos propuesta para el SIGR

## 1. Introducción

La estructura de datos permitirá organizar la información que utilizará el Sistema Integral de Gestión de Restaurante.

Para esta etapa se propone un modelo lógico que identifica las principales entidades y sus relaciones. Su finalidad es mostrar qué información necesitaría el sistema para gestionar usuarios, menú, pedidos, reservas y ventas.

Este modelo es documental y todavía no corresponde a una base de datos implementada.

## 2. Entidades principales

### 2.1 Usuarios

Almacenará los datos de las personas que tengan acceso al sistema.

Campos propuestos:
- id_usuario: identificador único.
- nombre: nombre de la persona.
- correo: dirección de correo electrónico.
- contrasena_hash: contraseña almacenada de forma protegida.
- rol: cliente, mesero o administrador.
- estado: indica si la cuenta está activa.

### 2.2 Categorías

Permitirá organizar los platos del menú.

Campos propuestos:
- id_categoria: identificador único.
- nombre: nombre de la categoría.
- descripcion: información complementaria.
- estado: disponibilidad de la categoría.

### 2.3 Platos

Contendrá la información de los productos ofrecidos por el restaurante.

Campos propuestos:
- id_plato: identificador único.
- id_categoria: categoría a la que pertenece.
- nombre: nombre del plato.
- descripcion: detalle del producto.
- precio: valor de venta.
- disponible: indica si puede solicitarse.

### 2.4 Pedidos

Registrará las solicitudes realizadas por los clientes.

Campos propuestos:
- id_pedido: identificador único.
- id_usuario: usuario relacionado con el pedido.
- fecha: fecha de registro.
- tipo_servicio: mesa, recogida o domicilio.
- estado: situación actual del pedido.
- total: valor total.

### 2.5 Detalle de pedidos

Permitirá identificar los platos y cantidades incluidos en cada pedido.

Campos propuestos:
- id_detalle: identificador único.
- id_pedido: pedido relacionado.
- id_plato: plato solicitado.
- cantidad: unidades solicitadas.
- precio_unitario: precio aplicado al momento del pedido.
- subtotal: valor de la línea.

### 2.6 Reservas

Almacenará las solicitudes de reserva de mesas.

Campos propuestos:
- id_reserva: identificador único.
- id_usuario: cliente relacionado.
- fecha_reserva: día solicitado.
- hora_reserva: hora solicitada.
- numero_personas: cantidad de asistentes.
- estado: situación de la reserva.

### 2.7 Pagos

Registrará los pagos asociados a los pedidos.

Campos propuestos:
- id_pago: identificador único.
- id_pedido: pedido relacionado.
- fecha_pago: fecha de la operación.
- valor: importe pagado.
- medio_pago: efectivo, tarjeta u otro medio habilitado.
- estado: situación del pago.

### 2.8 Cierres de caja

Permitirá conservar el resumen de las operaciones de una jornada.

Campos propuestos:
- id_cierre: identificador único.
- fecha_cierre: día de la operación.
- responsable: usuario encargado.
- total_ventas: suma de las ventas registradas.
- observaciones: comentarios del cierre.

## 3. Relaciones entre las entidades

- Una categoría puede tener varios platos.
- Un usuario puede registrar varios pedidos.
- Un pedido puede contener varios detalles.
- Cada detalle corresponde a un plato.
- Un usuario puede solicitar varias reservas.
- Un pedido puede tener uno o varios registros de pago, según las reglas que se definan para el sistema.
- Un cierre de caja reúne los pagos y ventas correspondientes al periodo revisado.

## 4. Consideraciones de diseño

Los identificadores permitirán diferenciar cada registro. Las relaciones entre entidades ayudarán a evitar la duplicación innecesaria de información.

Los precios de los platos deberán conservarse en el detalle del pedido para mantener el valor aplicado cuando se realizó la venta, incluso si el precio del menú cambia posteriormente.

Las contraseñas no deberán almacenarse como texto visible. Se deberá utilizar un mecanismo seguro de protección.

## 5. Alcance del modelo

Esta estructura representa una propuesta inicial para documentar la información del SIGR. Los campos y relaciones podrán ajustarse cuando se realice el diseño técnico y se seleccione el motor de base de datos.
