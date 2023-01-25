# Clase 02. Seguridad de la información

*Autor:* Daniel Arbeláez

*Creado:* 18/09/2022

*Docente:* Jhon Edison Rodriguez Guisado
***

## Tabla de contenido

- [Clase 02. Seguridad de la información](#clase-02-seguridad-de-la-información)
  - [Tabla de contenido](#tabla-de-contenido)
  - [Máquinas virtuales](#máquinas-virtuales)

## Máquinas virtuales

Los programnas más usados son vmware y virtualbox (virtualbox tiene una versión pro que tiene unas funcionalidades adicionales). Vamos a instalar la version Windows 10 Pro.

> Serial Activacion VmWare WorkStation Pro: ZF3R0-FHED2-M80TY-8QYGC-NPKYF.
> Algo muy importante de todas la maquinas de virtualización es entrar a la Bios y verificar si el sistema tiene activo el componente de virtualziación activo (Intel-VT, AMD-V)

Para el presente curso usaremos las siguientes ISO's:

- Kali Linux o Parrot OS
- Ubuntu
- Windows 7 Enterprise SP1

Otro software para hacer diagramas de infraestructura de empresas es [drawio](https://github.com/jgraph/drawio-desktop/releases) o si no se quiere instalar softwasre de puede usa la página [diagrams](https://www.diagrams.net) para hacer los mismo diagramas

Procedemos a descargar ubuntu server desde el siguiente [link](https://ubuntu.com/download/server). Hay otra versión de ubutu desktop que tiene la versión de escritorio.

- La nombramos como UbuntuServer; se le asigna de ram aproximadamente 1 gb para casos en los que se usan varias máquinas virtuales; usar tipo de disco duro VDI (Virtualbox= .VDI, Microsoft= .VHD, VmWare = .VMDK) al menos se le debe asignar unas **40 gb** al ubuntu server; usar la confirguración de disco Reservado dinámicamente.
- Instalamos en inglés
- Seleccionamos el server
- Desactivamos la opcion LVM group
- Activamos el sevicio OpenSSH (sirve para conectarse remotamente y hacer actualizaciones etc)
- Una vez aparezca Install complete, seleccionamos reboot now
- Puede aparecer un error por estar trabajando en maquina virtual seleccionar continuar

En linux un usuario básico se determina con el signo `$`, un usuario con privilegios o root aparece como `#`. Para cambiar a ausuario con privilegios se usa el comando `sudo su`. Seguido buscamos actualizaciones con el comando `apt update`, luego `apt upgrade`. Luego se habilitan los daemons. Para hacer una limpieza a nivel de sistema operativo se usa `apt autoremove`. Finalmente se reinicia y luego ya quedan operativas las nuevas funcionalidades. Para apagar el sistema se usa el comando `sudo poweroff`

Datos usados para maquina virtual:
user: nessus
pass: 1234

Actividad para lo próxima clase:

Debes realizar la investigacion y crear una presentacion sobre el tema elegido:

1. DevOps.
2. DevSecOps.
3. Zenoss Core.
4. Traefik.
5. Kubernetes.
6. Juniper Networks.
7. Docker.
8. ATP.
9. Symantec EndPoint Protection.
10. Symantec DLP.
11. Ubuntu Core.
12. **Raspberry Pi**.
13. Arduino.
14. Windows 10.
15. Windows 11.
16. Windows Server 2016.

Dentro de la investigacion, mencionar al menos una (01) vulnerabilidades identificada en esta plataforma/tecnologia.
Contar generalidades de la vulnerabilidad y la posible solucion.

***

Concepto [Raspberry Pi](https://es.wikipedia.org/wiki/Raspberry_Pi)

Búsqueda de vulnerabilidades de la raspberi pi [link](https://cve.mitre.org/cgi-bin/cvekey.cgi?keyword=raspberry+pi)

Link de interes sobre proyectos de hacking etico con raspberry pi y kali linux [link directo](https://gbhackers.com/raspberry-pi-and-kali-linux/)
