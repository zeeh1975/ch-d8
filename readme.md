## **Backend Coderhouse - Desafío 8 - Clase 16: Nuestra Primera Base de Datos**

**Consigna:** Tomando como base las clases Contenedor en memoria y en archivos, desarrollar un nuevo contenedor con idénticos métodos pero que funcione sobre bases de datos, utilizando Knex para la conexión. Esta clase debe recibir en su constructor el objeto de configuración de Knex y el nombre de la tabla sobre la cual trabajará. Luego, modificar el desafío entregable de la clase 11 ”Chat con Websocket”, y:
  - cambiar la persistencia de los mensajes de filesystem a base de datos SQLite3.
  - cambiar la persistencia de los productos de memoria a base de datos MariaDB.

Desarrollar también un script que utilizando knex cree las tablas necesarias para la persistencia en cuestión (tabla mensajes en sqlite3 y tabla productos en mariaDb).

**Notas:**
Definir una carpeta DB para almacenar la base datos SQLite3 llamada ecommerce

**Detalles del desafio:** 
- Utilizar **npm install** para descargar las dependencias.
- Primero para crear las bases de datos usar **node db/crearBases.js** Se asume que MariaDB esta funcionando en localhost puerto 3306 y el usuario "root" no tiene contraseña, si no fuera este el caso cambiar esos datos en ./options/mariadb.js
- Usar **node src/server.js** para ejecutar el proyecto
