# Creando-usuarios-y-grupos

//Para poder crear usuarios y grupos es necesario que accedamos en modo root

//se agrega el comando "sudo groupadd [nombre_de_grupo] para agregar el grupo deseado"

root@debian:~$ sudo groupadd casa

//para agregar "usuarios usamos sudo useradd [nombre]"

root@debian:~$ sudo useradd javierm
root@debian:~$ sudo useradd padres

//Para establecer una contraseña utilizamos "passwd [usuario]"

root@debian:~$ sudo passwd javierm
root@debian:~$ sudo passwd padres


//Para agregar los usuarios creados un grupo usamos "sudo adduser [nombre_del_usuario] [nombre_de_grupo]"

root@debian:~$ sudo adduser javierm casa


//Para realizar el cambio de nombre de un grupo existente usamos "sudo groupmod -n [Nuevo-nombre] [nombre_anterior]"

root@debian:~$ sudo groupmod -n Familia casa

//finalmente utilizamos "cat /etc/group para verificar" 

root@debian~$ cat /etc/group
