clear
apt update  
clear
apt install -y docker.io
docker --version
docker version
clear
apt install docker-compose -y
clear
10 docker-compose --v
docker-compose --version
clear
docker swarm init
docker service ls
docker nodes ls
docker node ls
clear 18
dokcer --version 19
clear
docker version
clear
docker pull hhtpd
clear  
docker pull httpd  
docker images  
docker run -it -d --name web1 -p 80:80 httpd:latest
docker ps
docker images -q  
docker rm -f web1
docker ps -a
docker ps
docker images
docker rm $(docker ps -aq)
docker rm -f $(docker ps -aq)
docker rm $(docker images -q)  
docker rmi -f $(docker images -q)
clear
docker service create --name myweb --replicas 3 nginx
docker service ls
docker service create --name myservice --mode global alpine top
docker service ls
docker services ps myservices
clear
docker service ps
docker service ps myweb  
docker service ps myservices
docker service ps myservice  
clear  
docker network ls  
docker network create -d overlay nginx-net1  
docker service create --name nginx-service1 --publish target=80,published-80 -replicas=5 --network nginx-net1 nginx
docker service create --name nginx-service1 --publish target=81,published-81 -replicas=5 --network nginx-net1 nginx
clear
docker pull
docker pull httpd  
docker run -it -d --name web1 -p 80:80 httpd:latest
docker ps  
clear
docker pull nginx
docker images  
docker run -it -d --name web2 -p 81:81 nginx:latest
docker ps
clear  
cd /var/lib/docker  
ls  
cd image
ls
cd overlay2
ls
cd overlay2  
cd imagedb  
ls  
cd metadata  
ls
cd sha256
ls
cd ..  
ls
cd ..  
ls  
cd content  
ls
cd sha256  
ls  
pwd  
cd ../../../  
ls  
cd ..
ls  
cd ..
clear  
ls
docker network sl  
docker network ls  
cd conatiners
cd containers  
ls  
cd 925d9be285473b36378c684cf6358a1a0b533511b7241ce642b980ee448c8f3a  
ls
ct hostanme  
cd hostname
clear
ls
cd ..  
cd ~
ls
clear  
docker images -q  
clear  
docker iamges
docker images  
docker rm -f nginx  
docker ps  
docker rm -f web1 web2
clear  
docker ps -a  
docker container kill -f 925d9be28547
docker container kill 925d9be28547  
clear
docker ps -a  
docker iamges  
docker images
ls  
clear  
docker images  
docker rmi -f dd34e67e3371 c8ca530172a8  
clear  
docker iamges  
docker images  
clear
docker service ls  
docker node ls  
docker service ps  
docker service ls
clear
docker network inspect nginx-net1  
sudo docker service create --name nginx-service1 --publish target=80,published=80 --replicas=5 --network nginx-net1 nginx
docker network inspect nginx-net1  
docker network inspect nginx-service1  
clear  
docker service inspect nginx-service1
docker rm nginx-net1  
docker network rm nginx-net1
docker service rm nginx-net1  
docker service rm nginx-service1  
docker network rm nginx-net1  
clear  
docker service ls  
docker service rm myweb
docker service rm myservice
clear  
docker ps  
docker ps -a
docker images  
docker images -q  
docker rmi -f $(docker images -q)  
clear   
docker network create -d overlay my-overlay   
docker service create --replicas=3 --name my-web --network my-overlay nginx -p 3000:3000  
clear   
docker images  
docker ps  
docker ps a-   
docker ps -a   
docker service rm my-web   
clear   
docker ps -a   
clear   
ls   
clear  
docker service create --replicas=3 --name my-web --network my-overlay nginx   
docker service ls   
dokcer service -o wide   
docker service -o wide   
clear   
docker service ls -o wide   
clear   
docker service ps my-web   
docker network inspect my-overlay   
docker service rm my-web  
clear   
docker service ls   
clear   
docker service create --mode global --publish mode=host,target=80,published=8080 --name nginx nginx:latest  
docker service ps nginx   
top   
clear   
docker service create --name my-web --replicas=3 --publish published=5050,target=80 nginx   
docker service ls   
docker service ps my-web   
docker service ps nginx   
docker service ps my-web   
docker service ps nginx   
clear   
docker swarm update --autolock=true   
systemctl docker restart   
service docker restart   
docker service ls   
docker swarm unlock   
docker service ls   
docker swarm unlock-key   
docker service ls   
docker swarm update --autolock=false   
clear   
docker service ls   
docker node ls   
clear   
docker service create --replicas=3 --name redis --update-deploy 10s redis:3.0.6   
sudo docker service create --replicas 3 --name redis --update-delay 10s redis:3.0.6   
docker service ps redis   
docker node update --availablity drain hostanme-worker1   
sudo docker node update --availability drain hostname_Worker1   
sudo docker node update --availability drain hostname_worker1   
clear   
sudo docker node update --availability drain ip-172.31.84.112   
sudo docker node update --availability drain ip-172-31-84-112   
clear   
sudo docker node update --availability drain ip-54-211-18-193   
clear   
docker node ls   
sudo docker node update --availability drain worker   
sudo docker node update --availability drain worker1   
sudo docker node inspect --pretty worker1   
docker service ps redis   
sudo docker node update --availability active worker1   
docker node inspect --pretty worker1   
docker service rm redis   
docker service ls   
docker service rm my-web nginx   
clear   
docker service create --name redis --replicas 3 redis:306   
docker service ls   
docker service rm redis   
clear   
docker service create --name redis --replicas 3 redis:3.0.6   
docker service ps redis   
docker inspect --pretty redis   
docker service inspect --pretty redis  
docker service inspect redis   
docker service rm redis   
history  
clear   
history > file.txt   
ls   
cat file.txt   
clear   
ls   
rm -rf file.txt   
clear   
docker service create --name redis --replicas 3 redis:3.0.6   
docker service ls   
docker node update --availbality drain worker1   
docker node update --availability drain worker1   
clear   
docker service create --name registry --publish published=5000,target=5000 registry:2   
docker service ls   
docker inspect registry | grep -i ipaddr   
docker inspect registry | grep ipaddr   
docker inspect registry   
curl 10.0.0.7:5000   
clear   
curl 10.0.0.7:5000/v2   
curl http://localhost:5000/v2/   
clear   
cd /home   
ls   
cd ubuntu   
ls   
mkdir stackdemo   
cd stackdemo   
ls   
nano app.py   
nano   
nano requirements.txt   
nano Dockerfile   
nano docker-compose.yaml   
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.1/docker-compose-$(uname-s)-$(uname -m)" -o /usr/-localbin/docker-compose   
docker-compose --version   
docker-compose up -d   
nano Dockerfile   
docker-compose up -d   
docker-compose ps   
docker-compose down --volumes   
docker-compose push   
docker stack deploy --compose-file docker-compose.yaml stackdemo   
docker stack services stackdemo   
curl localhost:5000   
curl http://localhost:8000   
clear  
docker service ls   
docker ervice scale redis=5   
docker service scale redis=5   
docker service update --replicas=4 registry   
docker service scale redis=4 registry=3   
docker service ls   
clear   
docker service create --mode global --name nginx nginx:latest   
docker service scale nginx=10   
clear   
docker volume ls   
docker volume create my_vol   
docker run -it -d --name web1 -v my_vol:/var/www/html nginx   
docker ps   
clear   
docker run -d --name myweb2 -mount src=my_vol,dst=/var/www/html nginx   
docker run -d --name myweb2 --mount src=my_vol,dst=/var/www/html nginx   
docker ps   
docker rm -f web1 myweb2   
docker ps -a   
clear   
ls   
docker run -d --name myweb1 -v type=bind,source="$(pwd)"/html,target=/var/www/html nginx  
docker ps  
docker ps -a  
docker rm -f web1  
docker rm -f myweb1  
clear  
sudo docker run -d --name myweb1 -v type=bind,source="$(pwd)"/html,target=/var/www/html nginx  
ls
sudo docker run -d --name myweb1 --mount type=tmpfs,destination=/app nginx  
sudo docker run -d --name myweb2 --mount type=tmpfs,destination=/app nginx  
docker rm myweb1 myweb2  
docker rm -f myweb2  
clear  
docker run -d --name myweb1 --mount type=tmpfs,destination=/app nginx  
docker ps  
docker run -d --name myweb2 --tmpfs /app nginx  
docker rm -f myweb1 myweb2  
clear
docker run -it --name webapp -v my_vol  
docker run -it --name webapp -v my_vol:/var/www/html alpine  
docker volume create volume1
docker service create -d --replicas=4 --name replicated-service --mount source=volume1.target=/app nginx:latest  
sudo docker service create -d --replicas=4 --name replicated-service --mount source=volume1,target=/app nginx:latest  
docker service ps replicated-service  
docker volume ls  
clear
nano /etc/docker/daemon.json  
sudo nano /etc/docker/daemon.json  
clear
docker info  
docker info | grep -i containers  
docker info | grep -i running  
docker info | grep -i stooped  
docker info | grep -i stopped  
clear  
docker info | grep -i driver  
docker node ls
docker services ls
docker service ls  
docker node update --availability --autolock=worker1
docker service ls  
clear  
history
docker node update --availability active worker1  
clear
docker node inspect worker1  
clear  
docker node update --label-add workernode1 worker1  
docker node update --label-add type=queue worker1
docker node update inspect worker1  
docker node update inspect workernode1  
clear  
docker node inspect worker1  
clear
docker service ls redis
docker service ls  
clear
docker service ls  
docker service inspect redis  
docker service ps redis
apt install jp  
docker inspect zv8h9l9nky44 | jq -r '.[].Status.ContainerStatus.ContainerID'  
apt install jqclea
cllear 376 clear  
docker inspect zv8h9l9nky44 | jq -r '.[].Status.ContainerStatus.ContainerID'  
docker inspect zv8h9l9nky44 | jq '.[].State'
docker inspect zv8h9l9nky44 | jq -r '.[].Status.ContainerStatus.ContainerID'
docker servicel 381 docker service ls
docker inspect onpzptfgmine | jq -r '.[].Status.ContainerStatus.ContainerID'  
clear  
docker service logs redis  
clear  
ifconfig  
apt install net-tools  
clear
ifconfig  
brctl show  
ip route show  
bridge fdb show
ipvsadm  
apt install ipvsadm  
ipvsadm  
net-stats -tnulp
clea
clear
netstat -ynulp
netstat -tnulp
clear
free -m
lscpu  
clear  
cd .ssh
cd ~  
clear
cd .ssh  
ls
nano authorized_keys  
chmod -R 700 .ssh  
cd ..  
clear
ssh ubuntu@172.31.84.112  
ssh ubuntu@ip-172.31.84.112  
ssh ubuntu@ip-172-31-84-112  
clear  
ssh ubuntu@worker  
ssh ubuntu@worker1  
clear  
ssh root@172-31-84-112  
ssh root@172.31.84.112  
clear  
ssh ubuntu@172.31.84.112  
ssh ubuntu@172-31-84-112  
clear  
nano .ssh/authorized_keys  
ssh ubuntu@172-31-84-112  
ssh root@172.31.84.112  
clear  
nano .ssh/authorized_keys  
ssh root@worker1  
clear  
ls  
history > docker-swarm-commands.md
