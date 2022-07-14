```
    1  mkdir 02-Dockerfile/apache/v1 -p 
    2  ls
    3  cd 02-Dockerfile/apache/v1/
    4  ls
    5  vim Dockerfile 
    6  ls
    7  docker build -t mywebapache:v1 . 
    8  docker images 
    9  docker inspect mywebapache:v1 
   10  docker history mywebapache:v1 
   11  docker images 
   12  docker run -d --name test-apache-1 mywebapache:v1
   13  docker ps 
   14  curl 172.17.0.2
   15  curl 172.17.0.3
   16  ls
   17  cd ..
   18  ls
   19  docker images 
   20  ls
   21  cp -rf v1 v2 
   22  ls
   23  cd v2/
   24  ls
   25  vim index.html
   26  ls
   27  mv Dockerfile apache-exp1
   28  ls
   29  vim apache-exp1 
   30  ls
   31  docker build -t mywebapache:v2 . 
   32  ls
   33  docker build -t mywebapache:v2 -f apache-exp1 . 
   34  docker images 
   35  docker run -d --name test-apache-2 mywebapache:v2
   36  docker ps 
   37  curl 172.17.0.3
   38  curl 172.17.0.4
   39  ls
   40  docker run -it --name test-apache-3 mywebapache:v2
   41  docker ps 
   42  ls
   43  cd ..
   44  ls
   45  cd ..
   46  ls
   47  history > README.md
```
