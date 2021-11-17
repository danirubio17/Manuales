
#Instalacion NextCloud

 1. Primero vamos a http://www.nextcloud.com le damos a /GetNextCloud/Server Packages y descargamos NextCloud.

 2. Lo primero que necesitamos es Apache2 y mysql

Entramos en un terminal y ejecutamos los siguientes comandos:


 Instalacion de Apache2:

   - apt update
   - apt upgrade
   - apt install -y apache2

Instalacion de mysql

   - apt update
   - apt upgrade
   - apt install -y mysql-server



Despues instalaremos unas librerias php que es el lenguaje principal que usan las aplicaciones.

   - apt install php libapache2-mod-php
   - apt install php-fpm php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-ldap php-zip php-curl



  3. Instalacion de una base de datos con mysql
---
    Creamos una base de datos.

      - CREATE DATABASE bbdd;
---
    Creamos un usuario

      - CREATE USER 'usuario'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
---

   Le damos privilegios al usuario

      - GRANT ALL ON bbdd.* to 'usuario'@'localhost';
---

   Salimos de la base de datos

      - exit
---
