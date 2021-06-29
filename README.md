# docker_comands_SLC
webpy, comandos docker save, docker load y COPY

## Comandos

## Ejecutar dockerfile
docker build -t webapp:v1 .

## Visualizar imagenes creadas
docker images

## Crear contenedor 
docker run -it -p 8080:8080 -v /workspace/docker_comands_SLC/docker:/docker --name webpy -h webpy webapp:v1

## Visualizar contenedor 
docker ps -a 
