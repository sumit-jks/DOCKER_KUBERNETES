```
311  mkdir 01-Apache
  312  cd 01-Apache/
  313  ls
  314  vim docker-compose.yaml
  315  ls
  316  docker-compose up -d
  317* docker ps
  318  docker-compose ps
  319  docker inspect 01-apache_nginx_1
  320  curl -vvv 172.17.0.4
  321  ls
  322  vim docker-compose.yaml
  323  docker-compose up -d
  324  docker-compose ps
  325  vim docker-compose.yaml
  326  docker images
  327  vim docker-compose.yaml
  328  ls
  329  cd ..
  330  ls
  331  cd ..
  332  ls
  333  cd 01-Docker-Basic/
  334  ls
  335  cd 02-Dockerfile/
  336  ls
  337  cd apache/
  338  ls
  339  cd v3/
  340  ls
  341  pwd
  342  cd ../../
  343  ls
  344  cd ..
  345  ls
  346  cd ..
  347  ls
  348  cd 02-DockerCompose/
  349  ls
  350  cd 01-Apache/
  351  ls
  352  vim docker-compose.yaml
  353  docker-compose up -d
  354  docker ps
  355  docker-compose ps
  356  cat docker-compose.yaml
  357  vim /root/docker-swarm-kuberenetes-ericsson-30-May-2022/01-Docker/01-Docker-Basic/02-Dockerfile/apache/v3/index.html
  358  docker-compose ps
  359  ls
  360  vim docker-compose.yaml
  361  docker-compose up -d
  362  docker-compose ps
```


```
 428  cd docker-swarm-kuberenetes-ericsson-30-May-2022/
  429  s
  430  ls
  431  cd 01-Docker/
  432  ls
  433  cd 02-DockerCompose/
  434  ls
  435  cd 02-Docker-Registry/ls
  436  ls
  437  cd 02-Docker-Registry/
  438  ls
  439  vim docker-compose.yaml
  440  docker-compose up -d
  441  docker network ls
  442  ls
  443  docker-compose  ps
  444  docker ps
  445  docker images
  446  docker tag 0e901e68141f master.example.com:8080/nginx
  447  docker images
  448  docker push master.example.com:8080/nginx
  449  docker images
  450  docker tag c5b0a79440ef master.example.com:8080/mywebapache:v1
  451  docker tag dc8bd4acd45e master.example.com:8080/mywebapache:v2
  452  docker tag 1e982f34d249 master.example.com:8080/mywebapache:v3
  453  docker tag 97ed6db29030 master.example.com:8080/mywebapache:v4
  454  docker images
  455  docker push master.example.com:8080/mywebapache:v1
  456  docker ps
  457  docker push master.example.com:8080/mywebapache:v2
  458  docker push master.example.com:8080/mywebapache:v3
  459  docker push master.example.com:8080/mywebapache:v4
  460  docker images
  461  nslookup master.example.com
  462  hosts master.example.com
  463  host master.example.com
  464  ping master.example.com
  465  docker push python-web-app:v2
  466  docker tag python-web-app:v2  amitvashist7/mypython-webapp-ericsson-01-june-2022:v2
  467  docker images
  468  docker push python-web-app:v2
  469  docker push amitvashist7/mypython-webapp-ericsson-01-june-2022:v2
  470  docker login
  471  docker push amitvashist7/mypython-webapp-ericsson-01-june-2022:v2
  472  docker run -d --name test-1 -P  172.31.0.100:8080/mywebapache:v4
  473  docker run -d --name test-1 -P  master.example.com:8080/mywebapache:v4
  474  docker pull master.exa mple.com:8080/mywebapache:v4
  475  docker pull master.example.com:8080/mywebapache:v4
  476  docker images
  477  docker rmi master.example.com:8080/mywebapache:v1
  478  docker pull master.example.com:8080/mywebapache:v1
  479  docker images
  480  docker tag 90337070264d amitvashist7/mypython-webapp-ericsson-01-june-2022:v1
  481  docker push amitvashist7/mypython-webapp-ericsson-01-june-2022:v1
  482  ls
  483  du -sh registry-data
  484  ls
  485  docker-compose ps
  486  docker-compose kill
  487  docker-compose ps
  488  docker-compose rm
  489  docker-compose ps
  490  docker ps -a
  491  ls
  492  rm -rf registry-data/
```
