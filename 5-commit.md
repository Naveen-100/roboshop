### 5 Commit {payment, ratings}
*** for i in web mongo catalogue  user cart mysql shipping ratings payment; do cd $i ; docker build -t $i:v1 . ; cd .. ; done

*** for i in web mongo catalogue  user cart mysql shipping ratings payment; do cd $i ; docker build -t $i:v1 . ; docker push naveen2809/$i:v1; cd .. ; done

* do payment for things in cart 
* payment depends on rabbitmq
* ratings depends on mysql
* docker build -t naveen2809/payment:v1 .
* docker build -t naveen2809/ratings:v1 .
* Enable payments, ratings proxy in web/default.conf
* docker build -t naveen2809/web:v1 .
* docker-compose up -d