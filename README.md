comandos-y-codigos
==================


MYSQL:
======
para volcar grandes cantidades de datos en mysql se ejecuta los siguientes commandos:

exportar del servidor.
mysqldump -u usuario -pcontraseña nombre-base-de-datos > fichero-exportacion.sql

importar al servidor.
mysql -u usuario -pcontraseña nombre-base-de-datos < fichero-importacion.sql


HTML
====

para las ñ y tildes:
<meta charset="utf8">


SHH
====

FTP
===
para descargar 
get


apache2
=======

remover todo el apache 
sudo apt-get purge --auto-remove apache2

instalar 
sudo apt-get install apache2

OpenPanel
========

aumentar las digueintes lineas en
/etc/apt/sources.list:
deb http://download.openpanel.com/deb/ <distribution> main
deb-src http://download.openpanel.com/deb/ <distribution> main

sudo -i

apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 4EAC69B9
apt-get update
aptitude install openpanel-suggested

para cambiar de contraseña
openpanel-cli
[openpanel]% password user openpanel-admin


