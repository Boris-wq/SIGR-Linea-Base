
# Procedimiento de control de cambios del SIGR

## 1. Introducción

Durante la organización de un proyecto de software pueden surgir nuevas necesidades o ajustes en las funciones que se habían definido inicialmente.

Por esta razón, el SIGR tendrá un procedimiento para revisar y registrar las modificaciones de su documentación. La intención es evitar cambios desordenados y conservar un historial que permita conocer cómo ha evolucionado el proyecto.

## 2. Objetivo

Establecer una forma de solicitar, analizar, aprobar y registrar los cambios realizados en los documentos que conforman la línea base del SIGR.

## 3. Tipos de cambios

Se tendrán en cuenta tres tipos principales:

- **Corrección:** ajustes de ortografía, redacción o errores encontrados en los documentos.
- **Mejora:** modificaciones que permiten explicar mejor una función o completar información.
- **Cambio funcional:** incorporación, eliminación o modificación de una característica del sistema.

## 4. Procedimiento para realizar un cambio

1. Identificar la necesidad de modificar un documento.
2. Describir el motivo del cambio.
3. Identificar los archivos y módulos afectados.
4. Revisar las consecuencias de la modificación.
5. Solicitar la revisión del responsable.
6. Realizar el ajuste cuando sea aprobado.
7. Registrar la modificación en GitHub mediante un commit.
8. Actualizar el CHANGELOG.md cuando corresponda.

## 5. Uso de GitHub

GitHub permitirá conservar el historial de los documentos.

Cada commit deberá tener un mensaje corto que explique el cambio realizado. Por ejemplo:

- docs: corregir descripcion del modulo de reservas
- docs: actualizar manual de usuario
- docs: ampliar criterios de la linea base

La rama main será la referencia principal del proyecto. Para modificaciones importantes se podrá trabajar en una rama independiente y solicitar una revisión antes de integrar los cambios.

## 6. Responsables

Los integrantes del equipo podrán identificar y proponer modificaciones.

El coordinador o responsable designado revisará los cambios que afecten la línea base y determinará si pueden incorporarse a la versión estable.

## 7. Registro de cambios

Cada modificación importante deberá quedar identificada con:

- Fecha del cambio.
- Documento afectado.
- Descripción de la modificación.
- Responsable.
- Identificador del commit.
- Estado de aprobación.

## 8. Consideración final

El control de cambios permitirá mantener organizada la documentación del SIGR. También facilitará consultar versiones anteriores y reconocer las modificaciones realizadas durante el desarrollo del proyecto.
