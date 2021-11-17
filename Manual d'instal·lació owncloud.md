
#Manual instalacion OwnCloud

  1. Para instalar OwnCloud necesitamos un contenedor.

  2. Para crear un contenedor debemos de ejecutar los siguientes comandos:
---
        Crear el contenedor:

        lxc launch ubuntu:20.04 elmeucontenidor
---

        Encender el contenedor:

        lxc start elmeucontenidor
---

        Ejecutar el contenedor:

        lxc exec elmeucontenidor bash
---

  3. Instalar Apache2 y mysql
---
      - apt update
      - apt upgrade
      - apt install apache2
      - apt install mysql-server
---

  4. Instalar algunas librerias en el contenedor
---
      - apt install php libapache2-mod-php
      - apt install php-fpm php-common php-mbstring php-xmlrpc php-soap php-gd php-xml php-intl php-mysql php-cli php-ldap php-zip php-curl
---    
