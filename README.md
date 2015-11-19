# Tecleras UV en NodeJS

Aplicación de las tecleras uv en nodejs para el ramo de desarrollo web.

##Instalación

instalar nodejs

en la consola:

````
cd carpeta_donde_esta_bajada_la_app
````

pueden arrastrar y soltar la carpeta en la terminal de cmd o de linux.

````
npm install
````

si dice que npm es un comando no reconocido, cerrar todas las terminales y volverlas a abrir, si sigue diciendo, reiniciar el pc.

````
npm install -g gulp
````

##Arrancar

````
gulp
````

La página estará en localhost:3000

##Base de datos

Instalar MySQL 5.6.x (es la que uso, aunque en teoría debería funcionar con 5.7.x, no lo he probado).

Loguearse como root

en la consola de mysql, pegar los siguientes comandos

````
create user 'teclerasuv'@'localhost' identified by 'desarrolloweb';
````

````
create database teclerasuv;
````

````
grant all privileges on teclerasuv.* to teclerasuv@'localhost';
````

````
exit;
````

En cmd usar:

````
mysql -u teclerasuv -p teclerasuv < archivo_dump.sql
````

Cuando pida contraseña, tipear: desarrolloweb

Usando el archivo dump de la carpeta data.

##Tests

No sirven. los probé para farmautomático xD

Sería bueno que se hagan acá :o lo documentaré si tengo tiempo.

Son test de "carga o no la página", cosas así xD "Test unitarios" se llaman. pero no creo que de para hacerlos sinceramente, es fácil, pero no da el tiempo para que aprendan tanto D:
