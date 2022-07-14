```
    1  mkdir 03-DockerSwarm/00-Setup
    2  mkdir 03-DockerSwarm/00-Setup -p
    3  ip addr 
    4  docker kill $(docker ps -qa)
    5  docker rm $(docker ps -qa)
    6  ip addr 
    7  docker network ls 
    8  docker network rm 02-docker-registry_registry-ui-net 03-docker-registry_registry-ui-net mybr0 mynet
    9  docker network ls 
   10  ifconfig 
   11  ls
   12  git config --list 
   13  ip addr 
   14  docker swarm init --help
   15  docker swarm init --advertise-addr 172.31.0.100
   16  docker info
   17  docker ps 
   18  docker ps -a
   19  docker node ls
``` 
