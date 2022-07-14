```
478  cd 04-Visualizer/
  479  ls
  480  cat docker-compose.yaml
  481  docker stack deploy  -c docker-compose.yaml visual
  482  docker stack  ls
  483  docker service ls
  484  docker service create --name my_web --replicas 3  amitvashist7/python-web-app
  485  docker service ls
  486  docker service ps my_web
  487  docker ps
  488  docker inspect 080a7d6805d8
  489  curl 172.17.0.2:8081
  490  curl 172.17.0.2:8081/info
  491  docker service create --name my_web_2 --replicas 3 --publish published=8005,target=8081  amitvashist7/python-web-app
  492  docker service ls
  493  docker service ps my_web_2
  494  cd
  495  docker service create --name tiny-web --replicas 3 --publish published=8001,target=80  amitvashist7/k8s-tiny-web:latest
  496  docker service ls
  497  docker service ps tiny-web
  498  docker service inspect  tiny-web
  499  docker service ps tiny-web
  500  docker service scale tiny-web=10
  501  docker service ps tiny-web
  502  docker service update tiny-web --image amitvashist7/k8s-tiny-web:2
  503  docker service update tiny-web --image amitvashist7/k8s-tiny-web:3
  504  docker service update --rollback --update-delay 0s  tiny-web
```
