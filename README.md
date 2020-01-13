# docker-ubuntu-nginx-php
Create an Nginx web server and test php config using the Ubuntu 18.04 image.


Clone repo.

cd docker-ubuntu-nginx-php

docker build -t ub-nginx-php-1 .

docker run -d -p 80:80 ub-nginx-php-1

docker exec <CONTAINERNAME> service php7.2-fpm start
  
docker exec <CONTAINERNAME> service nginx start  

Open browser to hostname or docker container ip and test connnection of webserver as well as php connection.
