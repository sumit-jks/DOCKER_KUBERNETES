```
    1  ls
    2  mkdir 03-Docker-Volumes 
    3  ls
    4  docker run -it -v /var/www/amit ubuntu:16.04 
    5  docker ps 
    6  docker volume ls 
    7  docker ps 
    8  docker inspect loving_colden
    9  docker exec -it  loving_colden ls -ltr /var/www/amit 
   10  ls -ltr /var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data
   11  docker exec -it  loving_colden cat  /var/www/amit/hello.txt 
   12  cat  /var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data/hello.txt
   13  pwd 
   14  pwd >> /var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data/hello.txt
   15  hostname -f 
   16  hostname -f >> /var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data/hello.txt
   17  date >> /var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data/hello.txt
   18  cat  /var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data/hello.txt
   19  docker exec -it  loving_colden cat  /var/www/amit/hello.txt 
   20  ls
   21  docker ps 
   22  docker kill loving_colden
   23  docker rm  loving_colden
   24  docker ps -a 
   25  docker volume ls 
   26  docker volume inspect c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c
   27  cat "/var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data"
   28  cat "/var/lib/docker/volumes/c90522df7afc1f4f7e6b38baa2248e52060837ccd518b0094a2b805890b4385c/_data/hello.txt" 
   29  mkdir amit 
   30  ls
   31  rm -rf amit/
   32  
   33  docker volume ;s 
   34  docker volume ls
   35  docker volume create my-app-vol 
   36  docker volume ls
   37  docker volume inspect my-app-vol
   38  docker run -it --name vol-test-1 --mount source=my-app-vol,targer=/amit ubuntu:16.04 
   39  docker run -it --name vol-test-2 --mount source=my-app-vol,target=/amit ubuntu:16.04 
   40  docker run -it --name vol-test-2 -v my-app-vol:/amit ubuntu:16.04 
   41  docker ps 
   42  docker inspect vol-test-2
   43  docker attach  vol-test-2
   44  cat /var/lib/docker/volumes/my-app-vol/_data/hello.txt 
   45  ls
   46  pwd 
   47  cd ..
   48  ls
   49  pwd
   50  docker run -it --name vol-test-3 -v /root/docker-swarm-kuberenetes-ericsson-30-May-2022:/amit ubuntu:16.04 
   51  ls
   52  cd 01-Docker/
   53  ls
   54  cd 03-Docker-Volumes/
   55  ls
   56  cat hello.txt 
   57  cd ../../
   58  docker run -it --name vol-test-4 -v /root/docker-swarm-kuberenetes-ericsson-30-May-2022:/amit:ro ubuntu:16.04 
   59  ls
   60  docker ps 
   61  docker kill $(docker ps -qa ) 
   62  docker rm $(docker ps -qa ) 
   63  cd 
   64  docker run -itd --name data -v /var/www/html/amit -v /var/log/amit -v /etc/amit -v /root/docker-swarm-kuberenetes-ericsson-30-May-2022:/myapp:ro ubuntu:16.04 
   65  docker ps 
   66  docker inspect data
   67  ls
   68  docker run -itd --name test-vol-1 --volume-from date busybox 
   69  docker run -itd --name test-vol-1 --volumes-from date busybox 
   70  docker run -itd --name test-vol-1 --volumes-from data busybox 
   71  docker run -itd --name test-vol-2 --volumes-from data busybox 
   72  docker run -itd --name test-vol-3 --volumes-from data busybox 
   73  docker run -itd --name test-vol-4 --volumes-from data busybox 
   74  docker ps 
   75  docker inspect test-vol-2
   76  docker inspect test-vol-4
   77  docker ps 
   78  docker attach test-vol-4
   79  docker attach test-vol-3
   80  docker attach test-vol-2
   81  ls
   82  cd docker-swarm-kuberenetes-ericsson-30-May-2022/
   83  ls
   84  cd 01-Docker/
   85  ls
   86  cd 03-Docker-Volumes/
   87  ls
   88  rm -rf hello.txt 
   89  ls
   90  history 
   91  history >> REDAME.md
```
