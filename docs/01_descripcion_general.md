
# Descripción general del Sistema Integral de Gestión de Restaurante (SIGR)

## 1. Presentación del proyecto

El Sistema Integral de Gestión de Restaurante (SIGR) es una propuesta de software web creada para organizar las actividades principales de un restaurante.

En muchos restaurantes algunas tareas se realizan de forma manual. Por ejemplo, los pedidos se anotan en papel, las reservas se llevan en agendas y las ventas se revisan al finalizar la jornada. Esto puede ocasionar confusiones y dificultar el seguimiento de la información.

Con el SIGR se busca reunir estas actividades en una sola plataforma. De esta manera, el personal podrá consultar y administrar la información desde un mismo lugar.

## 2. Objetivo del sistema

El objetivo principal es facilitar la gestión diaria del restaurante mediante herramientas que permitan administrar usuarios, consultar el menú, registrar pedidos, organizar reservas y llevar el control de los pagos y las ventas.

## 3. Usuarios del sistema

El sistema contempla tres tipos de usuarios:

### Cliente

Podrá consultar el menú digital, conocer los platos disponibles, realizar pedidos y solicitar reservas según las opciones habilitadas por el restaurante.

### Mesero

Podrá consultar el menú, registrar pedidos de los clientes y revisar el estado de las solicitudes. También podrá consultar la información necesaria para atender las mesas.

### Administrador

Tendrá acceso a las funciones de administración. Podrá gestionar los usuarios, actualizar el menú, supervisar los pedidos y las reservas y consultar la información de caja y ventas.

## 4. Módulos que conforman el sistema

El SIGR estará organizado en cinco módulos principales:

### 4.1 Autenticación de usuarios

Este módulo permite identificar a las personas que ingresan a la plataforma. Cada usuario tendrá un perfil con permisos determinados. Así se evita que una persona pueda acceder a opciones que no le corresponden.

### 4.2 Menú digital

En este espacio se podrá consultar la oferta gastronómica del restaurante. El administrador tendrá la posibilidad de agregar platos, modificar sus descripciones, actualizar precios y cambiar su disponibilidad.

### 4.3 Registro y seguimiento de pedidos

Este módulo permitirá registrar los productos solicitados por los clientes y consultar el estado de cada pedido. También facilitará el seguimiento durante la preparación y la entrega.

Cuando el restaurante ofrezca servicio a domicilio, se podrá identificar el pedido y consultar sus avances. El rastreo mediante GPS sería una función adicional que requeriría otro desarrollo.

### 4.4 Reservas por fecha y hora

Permitirá registrar las solicitudes de reserva de los clientes. Se tendrán en cuenta datos como la fecha, la hora y el número de personas. El personal podrá consultar las reservas y actualizar su estado.

### 4.5 Cierre de caja y reportes de ventas

Este módulo estará orientado al control de los ingresos del restaurante. Permitirá consultar los pagos asociados a los pedidos y reunir la información necesaria para realizar el cierre diario y revisar las ventas.

## 5. Funcionamiento general

El proceso comienza cuando el usuario ingresa a la plataforma. De acuerdo con su perfil podrá acceder a las opciones disponibles.

El cliente podrá consultar el menú y realizar una solicitud. El mesero apoyará el registro y la atención de los pedidos. Mientras tanto, el administrador tendrá acceso a las funciones de supervisión y control.

Cuando se complete una venta, la información del pago quedará relacionada con el pedido. Estos datos servirán posteriormente para el cierre de caja y la elaboración de los reportes.

## 6. Alcance del proyecto

Para esta primera etapa se documentarán los cinco módulos indicados en la guía de aprendizaje. También se establecerán los usuarios, las funciones generales y la organización de los documentos.

El desarrollo del código fuente y la puesta en funcionamiento de la página web no hacen parte de esta etapa documental.

## 7. Importancia de la documentación

Documentar el sistema permite que todos los integrantes tengan claridad sobre lo que se espera construir.

Además, facilita identificar los componentes del proyecto y mantener un registro de los cambios. Esta información será la base para organizar las siguientes etapas y controlar las versiones mediante Git y GitHub.
