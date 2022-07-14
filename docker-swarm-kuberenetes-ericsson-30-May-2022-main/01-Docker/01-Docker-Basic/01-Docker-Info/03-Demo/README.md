```
    1  cat /etc/resolv.conf 
    2  ping -c2 google.com
    3  docker images 
    4  docker tag b6f507652425 ubuntu:16.04
    5  docker images 
    6  docker run ubuntu:16.04 cat /etc/os-release 
    7  echo $SHELL 
    8  cat /etc/os-release 
    9  docker run -i ubuntu:16.04 
   10  docker run -it ubuntu:16.04 
   11  docker ps 
   12  docker container ls 
   13  docker container ls -a 
   14  docker start 958d01d1f16c
   15* docker ps
   16  docker container ls 
   17  docker attach 958d01d1f16c
   18  docker container ls 
   19  ls
   20  docker ps 
   21  docker kill 958d01d1f16c
   22  docker ps 
   23  docker ps -a 
   24  docker start 958d01d1f16c
   25* 
   26  docker attach 958d01d1f16c
   27  docker ps 
   28  docker exec -it 958d01d1f16c cat /etc/os-release 
   29  docker exec -it 958d01d1f16c ls -ltr /root
   30  docker exec -it 958d01d1f16c ls -ltr /root/AmitVashist
   31  docker exec -it 958d01d1f16c cat  /root/AmitVashist/hello.txt 
   32  docker ps 
   33  docker rename hopeful_goldwasser job1 
   34  docker ps 
   35  docker run -it --name job2 ubuntu:16.04 
   36  docker ps 
   37  docker exec -it job1 cat  /root/AmitVashist/hello.txt 
   38  docker run -it --name job2 ubuntu:16.04 
   39  docker run -it --name job3 ubuntu:16.04 
   40  docker ps 
   41  docker run -d --name test-1 ubuntu:16.04 
   42  docker ps 
   43  docker ps -a
   44  docker run -itd --name test-2 ubuntu:16.04 
   45  docker ps 
   46  docker run -d --name tiny-web amitvashist7/k8s-tiny-web
   47  docker ps 
   48  docker ps -l 
   49  docker inspect test-2
   50  docker inspect tiny-web
   51  docker ps 
   52  docker ps -a 
   53  docker ps -aq
   54  docker ps -q
   55  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' job1 
   56  docker inspect --format '{{.Name}} {{.NetworkSettings.IPAddress}}' $(docker ps -q)
   57  docker ps 
   58  docker rm $(docker ps -qa)
   59  docker kill $(docker ps -qa)
   60  docker rm $(docker ps -qa)
   61  docker ps -a 
```

Let's install some packages inside the container & playaround: 

```
   80  docker run -it --name test-1 ubuntu:16.04
```
```
root@<containerid> # ping -c2 google.com
root@<containerid> # apt-get update
root@<containerid> # apt-get install iputils-ping -y
root@<containerid> # ping -c2 google.com
```

```
   81  docker ps
   82  docker attach test-1
   83  docker ps
   84  docker start test-1
   85  docker exec -it test-1 ping -c2 google.com
```
