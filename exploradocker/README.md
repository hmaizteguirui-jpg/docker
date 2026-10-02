# Explora Docker

En esta práctica vamos a explorar tanto la aplicación Docker Desktop de windows y los comando más utilizados de Docker.

- [Explora Docker](#explora-docker)
  - [Indicaciones de entrega](#indicaciones-de-entrega)
  - [Antes de empezar](#antes-de-empezar)
  - [1. Contenedores](#1-contenedores)
  - [2. Imagenes](#2-imagenes)
  - [3. Volumenes](#3-volumenes)
  - [4. Administrando contendores](#4-administrando-contendores)


## Indicaciones de entrega

- Responde en este fichero con capturas o texto según se requiera.
- Utiliza el formato correcto para los bloques de comando si los hubiera
- Recuerda ir publicando los cambios de vez en cuando usando los comandos, ejemplo:
```bash
git add --all
git commit -m "ejericicios 2, 3, 4 y 5"
git push
```

## Antes de empezar

- Pon Docker en marcha y ejecuta el comando de docker compose en esta carpeta para levantar la maquina. 
```bash
docker-compose up -d
```

## 1. Contenedores

1.1 ¿ Dónde podemos ver los contendores en marcha en la aplicación Docker Desktop? (Captura)![alt text](image-1.png)

1.2 Para ver los contendores en marcha desde la terminal se usa el comando `docker ps`, ejecutalo. (Captura)![alt text](image-2.png)

1.4 ¿Qué muestra el comando `docker container`?muestra opciones de comando docker container![alt text](image-3.png)

1.5 ¿Qué muestra el comando `docker container ls`? muestra las maquinas que ahi en docker![alt text](image-4.png)

## 2. Imagenes

2.1 ¿Dónde podemos ver las imágenes que tenemos descargadas en la aplicación Docker Desktop? (Captura)![alt text](image-5.png)

2.2 ¿Qué muestra el comando `docker images`?las imagenes del docker![alt text](image-6.png)

2.3 ¿Qué muestra el comando `docker image ls` muestra las imagenes deldocker tambien
![alt text](image-7.png)
## 3. Volumenes

3.1 ¿Dónde podemos ver los volumenes que tenemos en la aplicación Docker Desktop?en docker-desktop en el apartau containers (Captura)![alt text](image-8.png)

3.2 ¿Qué vemos en Docker Desktop si entramos en uno de los volumenes disponibles? (Captura)
![alt text](image-9.png)
3.3 ¿Qué muestra el comando `docker volume`?
![alt text](image-10.png)
3.4 ¿Qué muestra el comando `docker volume ls`?![alt text](image-11.png)

## 4. Administrando contendores

4.1 Si entramos en un contendor, verémos las siguientes pestañas. Las más importantes son **Logs**, **Exec** y **Files**. Explica para qué crees que sirve cada una.
• Logs: Muestra el historial de eventos y mensajes de salida del contenedor. Sirve para monitorear el comportamiento de la aplicación y diagnosticar errores en tiempo real.
• Exec: Permite ejecutar comandos directamente dentro del contenedor. Abre una terminal para realizar configuraciones o pruebas internas.
• Files: Ofrece un explorador de archivos interno del contenedor. Sirve para ver, modificar, descargar o subir archivos dentro de su sistema de almacenamiento.
![alt text](image.png)


4.2 Si queremos ejecutar comandos dentro de un contendor podemos usar Docker Desktop o podemos utilizar el comando `docker exec`. 
![alt text](image-12.png)
Para abrir una terminal, podemos ejecutar el programa bash con el parámetro -it (t de terminal e i de Standard Input).


```bash
docker exec -it <NOMBRE CONTENDOR> bash
```

Ejecuta el comando y muestra una captura de la terminal dentro del contendor.


4.3 Apaga todos los contendores de este proyecto con el comando `docker compose down` (Captura)
![alt text](image-13.png)