```
 74  git add . ; git commit -m "01-Docker-Intro" ; git push
   75  docker images
   76  docker run ubuntu cat /etc/os-relase
   77  docker run ubuntu cat /etc/os-release
   78  docker run ubuntu:16.04 cat /etc/os-release
   79  docker images
   80  docker pull amitvashist7/nginx-web
   81  docker pull amitvashist7/nginx-web:v2
   82  docker run -d -p 5000:5000 --name myregistry registry:2
   83  docker ps
   84  docker inspect registry:2
   85  ls
   86  docker ps
   87  docker images
   88  netstat tulnp
   89  netstat -tulnp
   90  hostname
   91  hostname -f
   92  docker images
   93  docker tag 3fb5cabb6469 master.example.com:5000/busybox:v1
   94  docker images
   95  docker push master.example.com:5000/busybox:v1
   96  vim /etc/resolv.conf
   97  ping google.com
   98  ls
   99  history
  100  ls
  101  docker images
  102  docker rmi 3fb5cabb6469
  103* docker rm $(docker ps -qa )
  104  docker rmi busybox
  105  docker images
  106  docker rmi master.example.com:5000/busybox:v1
  107  docker images
  108  docker ps
  109  docker run  master.example.com:5000/busybox:v1  echo "Hello World"
  110  docker pull busybox
  111  docker images
  112  docker ps
  113  docker images
  114  docker tag d2e4e1f51132 master.example.com:5000/ubuntu:latest
  115  docker tag b6f507652425 master.example.com:5000/ubuntu:16.04
  116  ls
  117  docker images
  118  telnet master.example.com 5000
  119  docker ps
  120  docker push master.example.com:5000/ubuntu:latest
  121  docker push master.example.com:5000/ubuntu:16.04
  122  ls
  123  docker images
  124  docker rmi $( docker images -q)
  125  docker images
  126  docker rmi $( docker images -q)
  127  docker rmi $( docker images -q) --force
  128  docker images
  129  docker pull ubuntu
  130  docker pull amitvashist7/k8s-tiny-web:1
  131  docker ps
  132  hostname -f
  133  docker search master.example.com:5000/ubuntu
  134  docker pull master.example.com:5000/ubuntu:latest
  135  docker ps
  136  docker images
  137  docker run master.example.com:5000/ubuntu cat /etc/os-release
  138  docker run master.example.com:5000/ubuntu:16.04  cat /etc/os-release
  139  docker run master.example.com:5000/busybox  cat /etc/os-release
  140  docker run master.example.com:5000/busybox:v1  cat /etc/os-release
  141  docker images
  142  history  | grep -i "docker push "
  143  docker ps
  144  ls
  145  docker ps
  146  docker stop myregistry
  147  docker image s
  148  docker images
  149  docker run master.example.com:5000/ubuntu:16.04  cat /etc/os-release
  150  docker images
  151  docker ps -a
  152  docker ps | grep -o master
  153  docker ps | grep -i master
  154  docker ps -a | grep -i master
  155  docker ps -a | grep -i master | awk -F '{print $1}'
  156  docker ps -a | grep -i master | awk -F " " '{print $1}'
  157  docker rm $(docker ps -a | grep -i master | awk -F " " '{print $1}')
  158  docker ps
  159  docker ps -a
  160  ls
  161  docker images
  162  docker images | grep -i master | awk -F " " '{print $1}'
  163  docker rmi $(docker images | grep -i master | awk -F " " '{print $1}')
  164  docker images | grep -i master | awk -F " " '{print $1}'
  165  docker rmi $(docker images | grep -i master | awk -F " " '{print $1}')
  166  docker rmi $(docker images | grep -i master | awk -F " " '{print $1}') --force
  167  docker images | grep -i master | awk -F " " '{print $1}'
  168  docker images
  169  docker rmi master.example.com:5000/busybox:v1
  170  docker rmi master.example.com:5000/ubuntu:16.04
  171  docker ps
  172  docker images
  173  docker run master.example.com:5000/ubuntu:16.04  cat /etc/os-release
  174  docker ps
  175  docker ps -a
  176  docker start myregistry
  177  docker ps
  178  docker run master.example.com:5000/ubuntu:16.04  cat /etc/os-release
```
