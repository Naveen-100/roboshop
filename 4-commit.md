### 4 Commit {cart, shipping, mysql}
* add things to cart 
* shipping deponds on mysql
* docker build -t naveen2809/cart:v1 .
* docker build -t naveen2809/mysql:v1 .
* docker build -t naveen2809/shipping:v1 .
* Enable shipping proxy in web/default.conf
* docker build -t naveen2809/web:v1 .
* docker-compose up -d