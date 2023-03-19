### Second Commit {Added User service}
* docker build -t naveen2809/user .
* docker run -itd --name user --network roboshop naveen2809/user

* docker build -t web:v1 .
* docker run -itd --network roboshop --name web -p 8081:80  web:v1