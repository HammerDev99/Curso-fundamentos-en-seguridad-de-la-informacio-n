# Clase 04. Instalación de w7 y configuración de ubuntu server

*Autor:* Daniel Arbeláez

*Creado:* 24/09/2022

*Docente:* Jhon Edison Rodriguez Guisado
***

## Tabla de contenido

- [Clase 04. Instalación de w7 y configuración de ubuntu server](#clase-04-instalación-de-w7-y-configuración-de-ubuntu-server)
  - [Tabla de contenido](#tabla-de-contenido)
  - [Recursos necesarios](#recursos-necesarios)
  - [Comandos](#comandos)

Existe un comando en w7 poara eliminar la configuracion de red `ip config /release` y `ipconfig/renew` para actualizar la conexión

creacion de correos temporales [link](https://www.mailinator.com/)

## Recursos necesarios

Nessus para el escaneo de vulnerabilidades desde el Ubuntu server [nessus-essentials](https://es-la.tenable.com/products/nessus/nessus-essentials)

link de acceso al nessus
[https://nessus:8834/](https://nessus:8834/)
[(https://192.168.1.17:8834/)](https://192.168.1.17:8834/)

Conexión remota a la linea de comandos del ubuntu server[Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

## Comandos

Activar superusuario `sudo su`

buscar el archivo en el directorio del ubuntu server
`chmod +x nombredelarchivo.deb`

instalacion del nessus
`dpkg -i nombredelarchivo.deb`

activacion del nessus
`systemctl enable nessusd`

verificacion del estado del nessus
`systemctl status nessusd`

iniciar el servicio de nessus
`systemctl start nessusd`

> Comando para evitar errores del explorador de windows donde se borran caché y dns desde el cmd `ipconfig /flushdns`

solucionar error de instalacion nessus `/opt/nessus/sbin/nessuscli update`, `/opt/nessus/sbin/nessuscli update --all` y `/opt/nessus/sbin/nessuscli fetch --register SERIAL` (Your activation code for Nessus Essentials is:FUUM-MAHM-L3KN-HJ7B-WPM3)

¿Cómo identificar el puerto de acceso a la plataforma nessus?
