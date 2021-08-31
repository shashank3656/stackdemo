1  clear
    2  apt update
    3  clear
    4  apt install -y docker.io
    5  docker --version
    6  docker version
    7  clear
    8  apt install docker-compose -y
    9  clear
   10  docker-compose --v
   11  docker-compose --version
   12  clear
   13  docker swarm init
   14  docker service ls
   15  docker nodes ls
   16  docker node ls
   17  clear
   18  dokcer --version
   19  clear
   20  docker version
   21  clear
   22  docker pull hhtpd
   23  clear
   24  docker pull httpd
   25  docker images
   26  docker run -it -d --name web1 -p 80:80 httpd:latest
   27  docker ps
   28  docker images -q
   29  docker rm -f web1
   30  docker ps -a
   31  docker ps 
   32  docker images
   33  docker rm $(docker ps -aq)
   34  docker rm -f  $(docker ps -aq)
   35  docker rm $(docker images -q)
   36  docker rmi -f  $(docker images -q)
   37  clear
   38  docker service create --name myweb --replicas 3 nginx
   39  docker service ls
   40  docker service create --name myservice --mode global alpine top
   41  docker service ls
   42  docker services ps myservices
   43  clear
   44  docker service ps 
   45  docker service ps myweb
   46  docker service ps myservices
   47  docker service ps myservice
   48  clear
   49  docker network ls
   50  docker network create -d overlay nginx-net1
   51  docker service create --name nginx-service1 --publish target=80,published-80 -replicas=5 --network nginx-net1 nginx
   52  docker service create --name nginx-service1 --publish target=81,published-81 -replicas=5 --network nginx-net1 nginx
   53  clear
   54  docker pull
   55  docker pull httpd
   56  docker run -it -d --name web1 -p 80:80 httpd:latest
   57  docker ps
   58  clear
   59  docker pull nginx
   60  docker images
   61  docker run -it -d --name web2 -p 81:81 nginx:latest
   62  docker ps
   63  clear
   64  cd /var/lib/docker
   65  ls
   66  cd image
   67  ls
   68  cd overlay2
   69  ls
   70  cd overlay2
   71  cd imagedb
   72  ls
   73  cd metadata
   74  ls
   75  cd sha256
   76  ls
   77  cd ..
   78  ls
   79  cd ..
   80  ls
   81  cd content
   82  ls
   83  cd sha256
   84  ls
   85  pwd
   86  cd ../../../
   87  ls
   88  cd ..
   89  ls
   90  cd ..
   91  clear
   92  ls
   93  docker network sl
   94  docker network ls
   95  cd conatiners
   96  cd containers
   97  ls
   98  cd 925d9be285473b36378c684cf6358a1a0b533511b7241ce642b980ee448c8f3a
   99  ls
  100  ct hostanme
  101  cd hostname
  102  clear
  103  ls
  104  cd ..
  105  cd ~
  106  ls
  107  clear
  108  docker images -q
  109  clear
  110  docker iamges
  111  docker images
  112  docker rm -f nginx
  113  docker ps
  114  docker rm -f web1 web2
  115  clear
  116  docker ps -a
  117  docker container kill -f 925d9be28547
  118  docker container kill  925d9be28547
  119  clear
  120  docker ps -a
  121  docker iamges
  122  docker images
  123  ls
  124  clear
  125  docker images
  126  docker rmi -f dd34e67e3371 c8ca530172a8
  127  clear
  128  docker iamges
  129  docker images
  130  clear
  131  docker service ls
  132  docker node ls
  133  docker service ps
  134  docker service ls
  135  clear
  136  docker network inspect nginx-net1
  137  sudo docker service create --name nginx-service1 --publish target=80,published=80 --replicas=5 --network nginx-net1 nginx
  138  docker network inspect nginx-net1
  139  docker network inspect nginx-service1
  140  clear
  141  docker service inspect nginx-service1
  142  docker rm nginx-net1
  143  docker network rm nginx-net1
  144  docker service  rm nginx-net1
  145  docker service  rm nginx-service1
  146  docker network rm nginx-net1
  147  clear
  148  docker service ls
  149  docker service rm myweb
  150  docker service rm myservice
  151  clear
  152  docker ps
  153  docker ps -a
  154  docker images
  155  docker images -q
  156  docker rmi -f $(docker images -q)
  157  clear
  158  docker network create -d overlay my-overlay
  159  docker service create --replicas=3 --name my-web --network my-overlay nginx -p 3000:3000
  160  clear
  161  docker images
  162  docker ps
  163  docker ps a-
  164  docker ps -a
  165  docker service rm my-web
  166  clear
  167  docker ps -a
  168  clear
  169  ls
  170  clear
  171  docker service create --replicas=3 --name my-web --network my-overlay nginx 
  172  docker service ls
  173  dokcer service -o wide
  174  docker service -o wide
  175  clear
  176  docker service ls -o wide
  177  clear
  178  docker service ps my-web
  179  docker network inspect my-overlay
  180  docker service rm my-web
  181  clear
  182  docker service ls
  183  clear
  184  docker service create --mode global --publish mode=host,target=80,published=8080 --name nginx nginx:latest
  185  docker service ps nginx
  186  top
  187  clear
  188  docker service create --name my-web --replicas=3 --publish published=5050,target=80 nginx
  189  docker service ls
  190  docker service ps my-web
  191  docker service ps nginx
  192  docker service ps my-web
  193  docker service ps nginx
  194  clear
  195  docker swarm update --autolock=true
  196  systemctl docker restart
  197  service docker restart
  198  docker service ls
  199  docker swarm unlock
  200  docker service ls
  201  docker swarm unlock-key
  202  docker service ls
  203  docker swarm update --autolock=false
  204  clear
  205  docker service ls
  206  docker node ls
  207  clear
  208  docker service create --replicas=3 --name redis --update-deploy 10s redis:3.0.6
  209  sudo docker service create --replicas 3 --name redis --update-delay 10s redis:3.0.6
  210  docker service ps redis
  211  docker node update --availablity drain hostanme-worker1
  212  sudo docker node update --availability drain hostname_Worker1
  213  sudo docker node update --availability drain hostname_worker1
  214  clear
  215  sudo docker node update --availability drain ip-172.31.84.112
  216  sudo docker node update --availability drain ip-172-31-84-112
  217  clear
  218  sudo docker node update --availability drain ip-54-211-18-193
  219  clear
  220  docker node ls
  221  sudo docker node update --availability drain worker
  222  sudo docker node update --availability drain worker1
  223  sudo docker node inspect --pretty worker1
  224  docker service ps redis
  225  sudo docker node update --availability active worker1
  226  docker node inspect --pretty worker1
  227  docker service rm redis
  228  docker service ls
  229  docker service rm my-web nginx
  230  clear
  231  docker service create --name redis --replicas 3  redis:306
  232  docker service ls
  233  docker service rm redis
  234  clear
  235  docker service create --name redis --replicas 3  redis:3.0.6
  236  docker service ps redis
  237  docker inspect --pretty redis
  238  docker service inspect --pretty redis
  239  docker service inspect redis
  240  docker service rm redis
  241  history
  242  clear
  243  history > file.txt
  244  ls
  245  cat file.txt
  246  clear
  247  ls
  248  rm -rf file.txt
  249  clear
  250  docker service create --name redis --replicas 3 redis:3.0.6
  251  docker service ls
  252  docker node update --availbality drain worker1
  253  docker node update --availability drain worker1
  254  clear
  255  docker service create --name registry --publish published=5000,target=5000 registry:2
  256  docker service ls
  257  docker inspect registry | grep -i ipaddr
  258  docker inspect registry | grep  ipaddr
  259  docker inspect registry 
  260  curl 10.0.0.7:5000
  261  clear
  262  curl 10.0.0.7:5000/v2
  263  curl http://localhost:5000/v2/
  264  clear
  265  cd /home
  266  ls
  267  cd ubuntu
  268  ls
  269  mkdir stackdemo
  270  cd stackdemo
  271  ls
  272  nano app.py
  273  nano 
  274  nano requirements.txt
  275  nano Dockerfile
  276  nano docker-compose.yaml
  277  sudo curl -L "https://github.com/docker/compose/releases/download/\
1.29.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
  278  docker-compose --version
  279  docker-compose up -d
  280  nano Dockerfile
  281  docker-compose up -d
  282  docker-compose ps
  283  docker-compose down --volumes
  284  docker-compose push 
  285  docker stack deploy --compose-file docker-compose.yaml stackdemo
  286  docker stack services stackdemo
  287  curl localhost:5000
  288  curl http://localhost:8000
  289  clear
  290  docker service ls
  291  docker ervice scale redis=5
  292  docker service scale redis=5
  293  docker service update --replicas=4 registry
  294  docker service scale redis=4 registry=3
  295  docker service ls
  296  clear
  297  docker service create --mode  global --name nginx nginx:latest
  298  docker service scale nginx=10
  299  clear
  300  docker volume ls
  301  docker volume create my_vol
  302  docker run -it -d --name web1 -v my_vol:/var/www/html nginx
  303  docker ps
  304  clear
  305  docker run -d --name myweb2 -mount src=my_vol,dst=/var/www/html nginx
  306  docker run -d --name myweb2 --mount src=my_vol,dst=/var/www/html nginx
  307  docker ps
  308  docker rm -f web1 myweb2
  309  docker ps -a
  310  clear
  311  ls
  312  docker run -d --name myweb1 -v type=bind,source="$(pwd)"/html,target=/var/www/html nginx
  313  docker ps
  314  docker ps -a
  315  docker rm -f web1
  316  docker rm -f myweb1
  317  clear
  318  sudo docker run -d --name myweb1 -v type=bind,source="$(pwd)"/html,target=/var/www/html nginx
  319  ls
  320  sudo docker run -d --name myweb1 --mount type=tmpfs,destination=/app nginx
  321  sudo docker run -d --name myweb2 --mount type=tmpfs,destination=/app nginx
  322  docker rm myweb1 myweb2
  323  docker rm -f  myweb2
  324  clear
  325  docker run -d --name myweb1 --mount type=tmpfs,destination=/app nginx
  326  docker ps
  327  docker run -d --name myweb2 --tmpfs /app nginx
  328  docker rm -f myweb1 myweb2
  329  clear
  330  docker run -it --name webapp -v my_vol
  331  docker run -it --name webapp -v my_vol:/var/www/html alpine
  332  docker volume create volume1
  333  docker service create -d --replicas=4 --name replicated-service --mount source=volume1.target=/app nginx:latest
  334  sudo docker service create -d --replicas=4 --name replicated-service --mount source=volume1,target=/app nginx:latest
  335  docker service ps replicated-service
  336  docker volume ls
  337  clear
  338  nano /etc/docker/daemon.json
  339  sudo nano /etc/docker/daemon.json
  340  clear
  341  docker info
  342  docker info | grep -i containers
  343  docker info | grep -i running
  344  docker info | grep -i stooped
  345  docker info | grep -i stopped
  346  clear
  347  docker info | grep -i driver
  348  docker node ls
  349  docker services ls
  350  docker service ls
  351* docker node update --availability --aut worker1
  352  docker service ls
  353  clear
  354  history
  355  docker node update --availability active worker1
  356  clear
  357  docker node inspect worker1
  358  clear
  359  docker node update --label-add workernode1 worker1
  360  docker node update --label-add type=queue worker1
  361  docker node update inspect worker1
  362  docker node update inspect workernode1
  363  clear
  364  docker node inspect worker1
  365  clear
  366  docker service ls redis
  367  docker service ls
  368  clear
  369  docker service ls
  370  docker service inspect redis
  371  docker service ps redis
  372  apt install jp
  373  docker inspect zv8h9l9nky44 | jq -r '.[].Status.ContainerStatus.ContainerID'
  374* apt install jqclea
  375  cllear
  376  clear
  377  docker inspect zv8h9l9nky44 | jq -r '.[].Status.ContainerStatus.ContainerID'
  378  docker inspect zv8h9l9nky44 | jq '.[].State'
  379  docker inspect zv8h9l9nky44 | jq -r '.[].Status.ContainerStatus.ContainerID'
  380  docker servicel
  381  docker service ls
  382  docker inspect onpzptfgmine | jq -r '.[].Status.ContainerStatus.ContainerID'
  383  clear
  384  docker service logs redis
  385  clear
  386  ifconfig
  387  apt install net-tools
  388  clear
  389  ifconfig
  390  brctl show
  391  ip route show
  392  bridge fdb show
  393  ipvsadm
  394  apt install ipvsadm
  395  ipvsadm
  396  net-stats -tnulp
  397  clea
  398  clear
  399  netstat -ynulp
  400  netstat -tnulp
  401  clear
  402  free -m
  403  lscpu
  404  clear
  405  cd .ssh
  406  cd ~
  407  clear
  408  cd .ssh
  409  ls
  410  nano authorized_keys
  411  chmod -R 700 .ssh
  412  cd ..
  413  clear
  414  ssh ubuntu@172.31.84.112
  415  ssh ubuntu@ip-172.31.84.112
  416  ssh ubuntu@ip-172-31-84-112
  417  clear
  418  ssh ubuntu@worker
  419  ssh ubuntu@worker1
  420  clear
  421  ssh root@172-31-84-112
  422  ssh root@172.31.84.112
  423  clear
  424  ssh ubuntu@172.31.84.112
  425  ssh ubuntu@172-31-84-112
  426  clear
  427  nano .ssh/authorized_keys
  428  ssh ubuntu@172-31-84-112
  429  ssh root@172.31.84.112
  430  clear
  431  nano .ssh/authorized_keys
  432  ssh root@worker1
  433  clear
  434  ls
  435  history > docker-swarm-commands.md
