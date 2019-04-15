# HappyLibrary
System to manage books

Instrucciones para ejecutar


1) Descargar el archivo Library.zip, descomprimir y abrir proyecto


2) Correr el comando "composer install"


3) Copiar el .env.example y crear una archivo .env con el mismo contenido, 
hacer las siguientes modificaciones para la conexion a la base de
datos:


DB_CONNECTION=mysql

DB_HOST=127.0.0.1

DB_PORT=3306

DB_DATABASE=[NOMBRE DE LA BASE DE DATOS]

DB_USERNAME=[USUARIO DE LA BASE DE DATOS]

DB_PASSWORD=[CONTRASENA DE LA BASE DE DATOS]


4) Correr las migraciones con:

php artisan migrate


5) Correr los siguientes seeds:

php artisan db:seed --class=CategoriesSeeder

php artisan db:seed --class=UsersSeeder

php artisan db:seed --class=BooksSeeder (Este ultimo opcinal si se desean tener libros desde el inicio)
