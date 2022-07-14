```
    1  mkdir 04-Docker-Network
    2  ls
    3  docker network ls 
    4  docker network inspect e526f2b3e3ad
    5  ip addr 
    6  route -n 
    7  ip addr 
    8  docker network inspect e526f2b3e3ad
    9  ls
   10  docker images 
   11  docker run -d --name net-test-1 mywebapache:v1 
   12  docker run -d --name net-test-2 mywebapache:v2 
   13  docker run -d --name net-test-3 python-web-app:v1
   14  docker [s 
   15  docker ps 
   16  s
   17  ls
   18  cat 01-Docker-Info/02-Demo/ | grep -i format 
   19  cat 01-Docker-Info/02-Demo/*  | grep -i format 
   20  cat 01-Docker-Info/03-Demo/README.md  | grep -i format 
   21  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   22  docker network inspect e526f2b3e3ad
   23  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   24  docker kill net-test-2
   25  docker run -d --name net-test-4 python-web-app:v1
   26  docker run -d --name net-test-5 python-web-app:v1
   27  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   28  docker start net-test-2
   29  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   30  docker network inspect e526f2b3e3ad
   31  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   32  curl -vv 172.17.0.2
   33  curl -vv 172.17.0.3
   34  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   35  docker ps 
   36  curl -vv 172.17.0.3:8081
   37  curl -vv 172.17.0.6
   38  ip addr 
   39  netstat -tulnp 
   40  docker run -d --name net-test-6 -p 8081:8081 python-web-app:v1
   41  docker ps 
   42  netstat -tulnp 
   43  curl localhost:8081
   44  curl 172.31.0.100:8081
   45  docker ps 
   46  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   47  netstat -tulnp 
   48  systemctl status docker 
   49  docker run -d --name net-test-7 -p 80:8081 python-web-app:v1
   50  netstat -tulnp 
   51  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   52  docker ps 
   53  docker run -d --name net-test-8 -p 80:8081 python-web-app:v1
   54  docker ps 
   55  docker inspect python-web-app:v1
   56  docker ps 
   57  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   58  curl 172.17.0.2
   59  curl 172.17.0.3
   60  curl 172.17.0.3:8081
   61  docker images 
   62  netstat -tulnp 
   63  ls
   64  docker images 
   65  ls
   66  cd 02-Dockerfile/
   67  ls
   68  cd apache/
   69  ls
   70  cp -rf v2 v3
   71  ls
   72  cd v3/
   73  ls
   74  vim apache-exp1 
   75  ls
   76  docker images 
   77  docker build -t mywebapache:v3 -f apache-exp1 
   78  docker build -t mywebapache:v3 -f apache-exp1 .
   79  docker images 
   80  docker inspect mywebapache:v3 
   81  cd 
   82  ls
   83  docker images 
   84  docker run -d --name net-test-9 -P  mywebapache:v2 
   85  docker run -d --name net-test-10 -P  mywebapache:v3
   86  docker ps 
   87  ls
   88  cd docker-swarm-kuberenetes-ericsson-30-May-2022/01-Docker/02-Dockerfile/apache/
   89  ls
   90  cp -rf v3 v4 
   91  ls
   92  cd v4/
   93  ls
   94  vim apache-exp1 
   95  ls
   96  docker build -t mywebapache:v4 -f apache-exp1 .
   97  docker run -d --name net-test-11 -P  mywebapache:v4
   98  docker ps 
   99  telnet 172.31.0.100 32770
  100  telnet 172.31.0.100 32769
  101  ls
  102  cd ..
  103  ls
  104  cd ..
  105  ls
  106  cd python-web-app/
  107  ls
  108  cp -rf v1 v2
  109  cd v2/
  110  ls
  111  vim Dockerfile 
  112  ls
  113  docker build -t python-web-app:v2 .
  114  cd 
  115  docker images 
  116  docker run -d --name net-test-12 -P  python-web-app:v2 
  117  docker ps 
  118  ls
  119  cd docker-swarm-kuberenetes-ericsson-30-May-2022/
  120  ls
  121  cd 01-Docker/
  122  ls
  123  cd 04-Docker-Network/
  124  ls
  125  mkdir 01-Demo
  126  ls
  127  cd 01-Demo/
  128  ls
  129  history >> README.md 
```
