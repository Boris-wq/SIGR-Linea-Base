
# Definición de la línea base del SIGR

## 1. ¿Qué es la línea base?

La línea base es el conjunto de documentos que se toman como referencia para organizar y controlar un proyecto de software.

En el caso del Sistema Integral de Gestión de Restaurante (SIGR), permitirá identificar qué información ha sido revisada y cuál será utilizada como punto de partida para continuar el trabajo.

Su importancia está en que cualquier modificación posterior podrá compararse con la versión inicial. Así será más fácil reconocer los cambios y mantener un historial organizado.

## 2. Elementos que conforman la línea base

Para esta primera etapa se tendrán en cuenta los siguientes archivos:

| Archivo | Función |
|---|---|
| README.md | Presenta el proyecto y explica su propósito. |
| CHANGELOG.md | Registra los cambios realizados. |
| 01_descripcion_general.md | Explica el sistema y su alcance. |
| 02_modulos_funcionales.md | Describe los cinco módulos principales. |
| 03_manual_usuario.md | Explica los procedimientos previstos para cada usuario. |
| 04_linea_base.md | Define los elementos que conforman la línea base. |

Estos documentos permiten tener una visión general del proyecto y sirven como referencia para las siguientes etapas.

## 3. Identificación de la versión inicial

Se propone utilizar la identificación v1.0.0 para la primera versión documental del SIGR.

Esta versión se considerará estable cuando los documentos estén completos, hayan sido revisados y cuenten con la aprobación del responsable del proyecto.

La versión deberá quedar relacionada con un registro específico de Git. De esta manera será posible identificar qué archivos fueron incluidos y consultar su historial.

## 4. Criterios para establecer la línea base

Antes de aprobar la versión inicial se deberán revisar los siguientes aspectos:

- La descripción general del sistema debe estar completa.
- Los cinco módulos establecidos en la guía deben estar documentados.
- Los perfiles de cliente, mesero y administrador deben estar identificados.
- El manual debe explicar los procedimientos principales.
- Los archivos deben estar organizados en las carpetas correspondientes.
- El repositorio debe permitir consultar el historial de cambios.
- La documentación debe ser revisada por el equipo responsable.

## 5. Control de versiones mediante GitHub

GitHub será el espacio donde se conservarán los documentos del proyecto.

Cada modificación importante deberá registrarse mediante un commit. Este registro permitirá conocer qué archivo cambió y cuál fue el motivo de la modificación.

La rama main se utilizará como referencia principal del proyecto. Cuando se realicen cambios que afecten documentos aprobados, estos deberán revisarse antes de incorporarse a la versión estable.

## 6. Procedimiento para modificar la línea base

Cuando sea necesario realizar un cambio, se seguirá este procedimiento:

1. Identificar el documento que necesita modificarse.
2. Explicar el motivo del cambio.
3. Revisar si afecta otros módulos o documentos.
4. Realizar la modificación correspondiente.
5. Revisar que la información siga siendo coherente.
6. Registrar el cambio mediante un commit.
7. Actualizar el CHANGELOG.md cuando corresponda.

Si la modificación cambia elementos que ya fueron aprobados, será necesario revisar nuevamente la línea base.

## 7. Responsables de revisión y aprobación

La revisión estará a cargo de los integrantes del equipo de trabajo.

La aprobación final corresponderá al coordinador o a la persona que sea designada para esta responsabilidad.

Los datos de aprobación se completarán cuando se realice la revisión definitiva.

## 8. Registro de identificación y aprobación

- Nombre del proyecto: Sistema Integral de Gestión de Restaurante.
- Identificación: SIGR.
- Versión propuesta: v1.0.0.
- Repositorio: SIGR-Linea-Base.
- Plataforma de control: GitHub.
- Rama principal: main.
- Fecha de aprobación: Pendiente.
- Responsable de aprobación: Pendiente.
- Estado: En construcción y revisión documental.

## 9. Consideración final

La línea base documental permitirá que el equipo trabaje sobre una misma referencia y mantenga organizados los documentos del SIGR.

Su aprobación no significa que la aplicación web ya esté construida. Significa que la documentación inicial ha sido revisada y aceptada como referencia para continuar el proyecto.
