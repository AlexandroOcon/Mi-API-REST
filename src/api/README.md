# MI API REST con Strapi - README

## Descripción

Este proyecto representa una API REST CRUD básica creada con Strapi, Node.js y XAMPP. 
La API proporciona operaciones básicas en el recurso "posts".
A continuación, se detallan los recursos disponibles y las acciones CRUD asociadas.

## Recursos y Acciones CRUD


| Recurso                        | Descripción                                            |
| ------------------------------ | ------------------------------------------------------ |
| **GET /posts**                 | Recupera la lista de todos los posts disponibles.      |
| **GET /posts/{id}**            | Obtiene información detallada sobre un post específico.|
| **GET /posts/findOne**         | Encuentra un solo post basado en criterios específicos.|
| **POST /posts**                | Crea un nuevo post.                                    |
| **PUT /posts/{id}**            | Modifica totalmente un post existente.                 |
| **PATCH /posts/{id}**          | Modifica parcialmente un post existente.               |
| **DELETE /posts/{id}**         | Elimina (soft delete) un post específico.              |
| **GET /usuarios**              | Recupera la lista de todos los usuarios disponibles.   |
| **GET /usuarios/{id}**         | Obtiene información detallada sobre un usuario específico.|
| **GET /usuarios/findOne**      | Encuentra un solo usuario basado en criterios específicos.|
| **POST /usuarios**             | Crea un nuevo usuario.                                 |
| **PUT /usuarios/{id}**         | Modifica totalmente un usuario existente.              |
| **PATCH /usuarios/{id}**       | Modifica parcialmente un usuario existente.            |
| **DELETE /usuarios/{id}**      | Elimina (soft delete) un usuario específico.           |
| **GET /actividades**           | Recupera la lista de todas las actividades disponibles.|
| **GET /actividades/{id}**      | Obtiene información detallada sobre una actividad específica.|
| **GET /actividades/findOne**   | Encuentra una sola actividad basada en criterios específicos.|
| **POST /actividades**          | Crea una nueva actividad.                              |
| **PUT /actividades/{id}**      | Modifica totalmente una actividad existente.          |
| **PATCH /actividades/{id}**    | Modifica parcialmente una actividad existente.        |
| **DELETE /actividades/{id}**   | Elimina (soft delete) una actividad específica.        |
| **GET /editoriales**           | Recupera la lista de todas las editoriales disponibles.|
| **GET /editoriales/{id}**      | Obtiene información detallada sobre una editorial específica.|
| **GET /editoriales/findOne**   | Encuentra una sola editorial basada en criterios específicos.|
| **POST /editoriales**          | Crea una nueva editorial.                              |
| **PUT /editoriales/{id}**      | Modifica totalmente una editorial existente.          |
| **PATCH /editoriales/{id}**    | Modifica parcialmente una editorial existente.        |
| **DELETE /editoriales/{id}**   | Elimina (soft delete) una editorial específica.        |
| **GET /libros**                | Recupera la lista de todos los libros disponibles.     |
| **GET /libros/{id}**           | Obtiene información detallada sobre un libro específico.|
| **GET /libros/findOne**        | Encuentra un solo libro basado en criterios específicos.|
| **POST /libros**               | Crea un nuevo libro.                                   |
| **PUT /libros/{id}**           | Modifica totalmente un libro existente.               |
| **PATCH /libros/{id}**         | Modifica parcialmente un libro existente.             |
| **DELETE /libros/{id}**        | Elimina (soft delete) un libro específico.            |
| **GET /inventario**            | Recupera la lista de todos los elementos en inventario.|
| **GET /inventario/{id}**       | Obtiene información detallada sobre un elemento en inventario específico.|
| **GET /inventario/findOne**    | Encuentra un solo elemento en inventario basado en criterios específicos.|
| **POST /inventario**           | Crea un nuevo elemento en inventario.                 |
| **PUT /inventario/{id}**       | Modifica totalmente un elemento en inventario existente.|
| **PATCH /inventario/{id}**     | Modifica parcialmente un elemento en inventario existente.|
| **DELETE /inventario/{id}**    | Elimina (soft delete) un elemento en inventario específico.|

### Instalación

1. Clona este repositorio: `git clone https://github.com/AlexandroOcon/Mi-API-REST.git`
2. Navega a la carpeta del proyecto: `cd Mi-API-REST`
3. Instala las dependencias: `npm install`

### Configuración de Strapi
Antes que nada recordar que se necesitan varias cosas para abrir Strapi primero:

1. Instalar Node.js y npm
Asegúrate de tener Node.js y npm instalados en tu sistema. Puedes descargar e instalar Node.js desde https://nodejs.org/.

2. Vamos a ejecutar npx create-strapi-app@latest "my-project" en el CMD de nuestra carpeta esto simplemente escribiendo cmd en la barra
superior o ruta de acceso una vez ya con el codigo realizara unas preguntas pero antes instala XAMPP.

3. Instalar XAMPP y enlazarlo con Strapi:

Descarga e instala XAMPP desde https://www.apachefriends.org/index.html.
Iniciar Servidores de Apache y MySQL:

Abre XAMPP y haz clic en los botones "Start" para los servicios de Apache y MySQL.
Acceder a phpMyAdmin:

Abre tu navegador web y visita http://localhost/phpmyadmin/.
Inicia sesión con el usuario y contraseña predeterminados (por lo general, root sin contraseña).
Crear una Base de Datos para Strapi:

En la interfaz de phpMyAdmin, crea una nueva base de datos. Por ejemplo, puedes llamarla strapi.
Configurar Strapi para Usar XAMPP:

Cuando configuras Strapi, especifica la información de conexión a la base de datos utilizando custom:
Tipo de base de datos: MySQL (u otro si estás utilizando otro sistema).
Host: localhost que siempre es el que te da predeterminado
Nombre de la base de datos: El nombre que le diste a la base de datos en phpMyAdmin (por ejemplo, strapi).
Usuario: root (u otro si has configurado un usuario diferente).
Contraseña: La contraseña que has establecido o dejado en blanco.

### Iniciar Strapi

npm run develop
