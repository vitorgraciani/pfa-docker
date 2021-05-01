# pfa-docker
Estudos docker


Criar rede

docker network create -d bridge  mynet

docker run  --rm --network mynet --name pfa-mysql -d vitorag/pfa-mysql

docker run --rm --network mynet --name pfa-golang -d vitorag/pfa-golang

docker run --rm  --network mynet --name pfa-nginx -p 8080:80 vitorag/pfa-nginx
