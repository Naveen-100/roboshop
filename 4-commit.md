### 4 Commit {cart, shipping, mysql}
* add things to cart 
* shipping deponds on mysql
* docker build -t cart:v1 .
* docker build -t mysql:v1 .
* docker build -t shipping:v1 .
* Enable shipping proxy in web/default.conf
* docker build -t web:v1 .
* docker-compose up -d