# README

Estos laboratorios correr en [Docker](https://docs.docker.com/engine/install/) y [Docker-compose](https://docs.docker.com/compose/install/) lo unico que se debe hacer es seguir las instrucciones de instalacion de la pagina oficial.

Para correr la interfaz grafica para docker solamente debemos correr el docker-compose.yml que de encuentra adentro con el siguiente comando.

```shell
agustin@debian:~$ cd Porteiner
agustin@debian:~/Porteiner# docker-compose up -d
```
> Tenga en cuenta que el puerto es el 3000 y el volumen esta montado para linux, de correr en windows debe montar el volumen correspondiente