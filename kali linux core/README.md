# README

Estos laboratorios correr en [Docker](https://docs.docker.com/engine/install/) y [Docker-compose](https://docs.docker.com/compose/install/) lo unico que se debe hacer es seguir las instrucciones de instalacion de la pagina oficial.

Las maquinas de Kali que estan configuradas no son necesarias para las auditorias, sos libre de usar cualquier sistema operativo. Pero si queres usarlas podes hacerlo entrando a la carpeta Kali-Linux y elegir cualquier version de linux que te parezca adecuada.

Por ejemplo si elegimos la version core, que es la más pequeña, abrimos una terminal y corremos el comando

```shell
agustin@debian:~$ cd L/Kali-Linux/core/
agustin@debian:~/L/Kali-Linux/core$ docker build .
```

Esto nos permitira instalar el Dockerfile configurado con esta version de kali. Si tenes dudas busca "como correr un Dockerfile".

kali-linux-core: Base Kali Linux System – core items that are always included

- cifs-utils
- ftp
- gdisk
- iw
- lvm2
- mlocate
- netcat-traditional
- nfs-common
- openssh-server
- openvpn
- p7zip-full
- parted
- rfkill
- samba
- snmp
- sudo
- tcpdump
- testdisk
- tftp
- tightvncserver
- tmux
- unrar
- vim
- whois
