# Clase 06

*Autor:* Daniel Arbeláez

*Creado:* 01/10/2022

*Docente:* Jhon Edison Rodriguez Guisado
***

## Tabla de contenido

- [Clase 06](#clase-06)
  - [Tabla de contenido](#tabla-de-contenido)
  - [Configuración final del Nessus](#configuración-final-del-nessus)
  - [Procedimiento en la plataforma](#procedimiento-en-la-plataforma)

## Configuración final del Nessus

Actualizaciones de nessus:
`apt update`

Eliminar librerias innecesarias como borrar los temporales (limpiar la casa):
`apt autoremove`

Actualización del nessus:
`/opt/nessus/sbin/nessuscli update`

Verificamos que el nesus tenga mínimo 3 gb de ram y reiniciamos el servidor:
`poweroff`

## Procedimiento en la plataforma

Ingresamos al nessus desde el navegador a la dirección `https://192.168.1.17:8834/` y una vez verificada la respuesta mediante el comando `ping` entre el servidor y el w7 seguido vamos a escaneos del nessus y seleccionamos "Nuevo" y luego en "Advanced scan".

En "Basic/General" ingresamos la ip del w7.

En "Basic/Schedule" se puede configurar una fecha, hora y frecuencia determinada para su ejecución.

En "Discovery/Host Discovery" se habilita ICMP y UDP

Entre otras configuraciones.

Con los puertos encontrados se puede buscar en el cmd

`ip:puerto`
