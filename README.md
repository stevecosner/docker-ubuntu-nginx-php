# docker-ubuntu-nginx-php
Create a web server and test php config with phpinfo page using the Ubuntu 18.04 docker container image and nginx.

Clone repo.

cd docker-ubuntu-nginx-php

docker build -t ubuntu-nginx-php-1 .

docker run -d -p 80:80 ubuntu-nginx-php-1

docker exec <CONTAINERNAME> service php7.0-fpm start
  
docker exec <CONTAINERNAME> service nginx start

Open browser to hostname or docker container ip and test connnection of webserver as well as php connection.


