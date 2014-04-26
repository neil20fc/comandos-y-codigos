comandos-y-codigos
==================
para volcar grandes cantidades de datos en mysql se ejecuta los siguientes commandos:

exportar del servidor.
mysqldump -u usuario -pcontraseña nombre-base-de-datos > fichero-exportacion.sql
importar al servidor.
mysql -u usuario -pcontraseña nombre-base-de-datos < fichero-importacion.sql

