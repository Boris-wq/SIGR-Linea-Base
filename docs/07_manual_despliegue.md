
# Manual de despliegue documental del SIGR

## 1. Introducción

Este documento explica cómo consultar y organizar la documentación del Sistema Integral de Gestión de Restaurante en el repositorio de GitHub.

Como el proyecto se encuentra en una etapa documental, este procedimiento corresponde a la publicación y consulta de los archivos. No representa la instalación de una aplicación web en un servidor.

## 2. Requisitos

Para consultar el repositorio se necesita:

- Un equipo con conexión a internet.
- Un navegador web actualizado.
- Acceso al repositorio de GitHub.
- Una cuenta de GitHub si se van a proponer modificaciones.

Para trabajar con Git de manera local también será necesario instalar Git en el equipo.

## 3. Consulta desde GitHub

1. Abrir el navegador.
2. Ingresar a GitHub.
3. Acceder al repositorio SIGR-Linea-Base.
4. Seleccionar la rama main.
5. Abrir la carpeta docs.
6. Seleccionar el documento que se desea consultar.

## 4. Clonar el repositorio

Si se desea disponer de una copia local de los documentos, se puede utilizar el siguiente comando:

git clone https://github.com/Boris-wq/SIGR-Linea-Base.git

Después se debe ingresar a la carpeta descargada:

cd SIGR-Linea-Base

## 5. Consultar el estado del repositorio

Para revisar los cambios realizados en la copia local se pueden utilizar estos comandos:

git status

Para consultar el historial:

git log --oneline

Para actualizar la copia local con los cambios publicados:

git pull

## 6. Publicación de modificaciones

Cuando una persona autorizada realice cambios en los documentos desde una copia local, deberá revisar los archivos y registrar las modificaciones.

Los comandos básicos son:

git add .
git commit -m "docs: actualizar documentacion SIGR"
git push

Los cambios deberán respetar el procedimiento de control definido para el proyecto.

## 7. Consideración sobre el despliegue de la aplicación

La página web del restaurante no se encuentra implementada en esta etapa. Por lo tanto, todavía no es posible documentar una instalación real, configurar un servidor o ejecutar la aplicación.

Cuando se desarrolle el software, será necesario complementar este manual con los requisitos técnicos, la configuración del entorno, la conexión con la base de datos y los pasos para publicar la aplicación.

## 8. Resultado esperado

Con este procedimiento los integrantes podrán consultar los documentos del proyecto, descargar una copia y mantener organizada la información mediante Git y GitHub.
