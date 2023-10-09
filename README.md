# APAGAR SERVICIO SWARM

docker swarm leave --force

# ENCENDER SERVICIO SWARM 

docker swarm init

# CONTRUIR LA IMAGEN BASADA EN DOCKERFILE (ubicarse en la carpeta donde esta el dockerfile)

docker build . -t nodeelena

# DESPLECAR EL SERVICIO CONFIGURADO EN EL DOCKER COMPOSE (ubicarse en la carpeta donde esta el docker-compose)

docker stack deploy -c docker-compose.yml miservicio

# ESCALAR EL SERVICIO (replicar el mismo contenedor x veces)

docker service scale miservicio_node=5
# proyecto_swarm_semi
