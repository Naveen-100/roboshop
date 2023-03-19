### First Commit {Dealing with web & catalogue}
* install git
* install docker
* add ec2-user to docker group
* clone repo: git clone https://github.com/instana/robot-shop.git
* create network in docker by
* docker network create roboshop
* docker build -t naveen2809/mongo:v1 .
* docker build -t naveen2809/catalogue:v1 .
* docker build -t naveen2809/web:v1 .
* docker run -d --name mongodb --network roboshop naveen2809/mongo:v1
* docker run -d --name catalogue --network roboshop naveen2809/catalogue:v1
* docker run -d --name web --network roboshop -p 80:80 naveen2809/web:v1
* docker ps
* docker ps -a