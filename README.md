**Foro Hub: API de Foro de Alura**
--------------------------------

**Introducción**
---------------

Esta API es un proyecto de desarrollo de una API REST para un foro de discusiones en línea. Se basa en los siguientes requerimientos:

* Crear una API REST para un foro que permita a los usuarios crear tópicos con dudas o sugerencias.
* Permite a otros usuarios responder e interactuar en los tópicos.

**Requerimientos**
-----------------

### Endpoints

* **GET /tópicos**: Listar todos los tópicos.
* **POST /tópicos**: Crear un nuevo tópico.
* **DELETE /tópicos/{id}**: Eliminar un tópico específico.
* **POST /auth**: Autenticación de usuarios (login).

### Campos para la creación de tópicos (POST /tópicos)**

* **id**: ID de la persona usuaria.
* **mensaje**: Mensaje del tópico.
* **nombre del curso**: Nombre del curso al que se refiere el tópico.
* **título**: Título del tópico.

### Autenticación y seguridad

* **Implementar seguridad utilizando tokens JSON Web (JWT)**.
* **Solo permitir que usuarios autenticados creen, actualicen o eliminen tópicos**.
* **Utilizar un endpoint de autenticación (/auth) para generar tokens JWT**.

### Base de datos

* **Utilizar una base de datos de tu elección para almacenar los datos del foro**.
* **Asegurarse de que los usuarios estén registrados en la base de datos antes de poder autenticarse**.

### Códigos de estado HTTP

* **200 OK**: Para listar tópicos exitosamente.
* **201 Created**: Para la creación exitosa de un tópico.
* **403 Forbidden**: Para indicar que el usuario no tiene permisos para realizar la acción.

### Herramientas

* **Insomnia (o similar)** para probar la API REST.
* **Trello (o similar)** para gestionar las tareas y el progreso del desarrollo.
