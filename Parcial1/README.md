

#### detener los contenedores con el comando
`$ docker-compose down`
#### Borrar los contenedores con el comando
`docker rm -f $(docker ps -a -q)`
#### Borrar  los volumenes con el comando
`docker volume rm $(docker volume ls -q)`
#### Reiniciar los contenedores con el comando:
`docker-compose up -d`

# Integrantes

Integrantes del equipo:
-ALEJANDRA MICHELLE MEJIA RIVAS MR22035
----IVAN EDUARDO LOPEZ TOBAR LT22009
-----ERICK GIOVANNI MONROY LOPEZ ML22048

parcial 1

$ docker-compose down

Borrar todos los contenedores con el comando:
docker rm -f $(docker ps -a -q)

Borrar todos los volumenes con el comando:
docker volume rm $(docker volume ls -q)

Reiniciar los contenedores con el comando:
docker-compose up -d

