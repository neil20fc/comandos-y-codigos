comandos-y-codigos
==================

Ubuntu
=======

apt-get update

apt-get upgrade

sudo apt-get dist-upgrade

tar
=====
tar xvf archivo.tar

MYSQL:
======
para volcar grandes cantidades de datos en mysql se ejecuta los siguientes commandos:

exportar del servidor.
mysqldump -u usuario -pcontraseña nombre-base-de-datos > fichero-exportacion.sql

importar al servidor.
mysql -u usuario -pcontraseña nombre-base-de-datos < fichero-importacion.sqlHow to Backup a MySQL Database

To backup a MySQL database, the database first has to exist in the database server and you have access to that server as well. You can use SSH or Telnet to login to the remote server if you do not have remote desktop to it. The command to backup a MySQL database as follows:


1
mysqldump -u [username] –p[password] [database_name] > [dump_file.sql]
The parameter of the command above as follows:

[username]: valid MySQL username.
[password]: valid password for the user. Note that there is no space between –p and the password.
[database_name]: database name you want to backup
[dump_file.sql]: dump file you want to generate.
By executing the above command all database structure and data will be exported into a single [dump_file.sql] dump file. For example, in order to back our sample database classicmodels, we use the following command:


1
mysqldump -u mysqltutorial –psecret  classicmodels > c:\temp\backup001.sql
How to Backup MySQL Database Structure Only

If you only want to backup database structure only you just need to add an option –no-data to tell mysqldump that only database structure need to export as follows:


1
mysqldump -u [username] –p[password] –no-data [database_name] > [dump_file.sql]
For example to backup our sample database with structure only, you use the following command:


1
mysqldump -u mysqltutorial –psecret  -no-data classicmodels > c:\temp\backup002.sql

mysqldump -u [username] –p[password] –no-create-info [database_name] > [dump_file.sql]


HTML
====

para las ñ y tildes:
<meta charset="utf8">


SHH
====
ssh login:contraseña@Maquina-a-la-que-queremos-conectarnos 

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


PHPMYADMIN
===========

para instalcion 

sudo apt-get install phpmyadmin

sudo gedit /etc/apache2/httpd.conf

Include /etc/phpmyadmin/apache.conf 

sudo /etc/init.d/apache2 restart 



SCP
===
copiar documentos de un a entre servidores
scp -r(si son mas de un archivo) usuario1@ip1:direc1  usuraio2@ip2@direc2







