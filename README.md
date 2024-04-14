# parcial_1DAW_GT1
Proyecto del parcial 1

$ docker-compose down

Borrar todos los contenedores con el comando:
docker rm -f $(docker ps -a -q)

Borrar todos los volumenes con el comando:
docker volume rm $(docker volume ls -q)

Reiniciar los contenedores con el comando:
docker-compose up -d
