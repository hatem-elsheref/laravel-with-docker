# laravel-with-docker
# DOCKER PHP & MYSQL & NGINX & LARAVEL

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](#)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](#)

# New Features!

  - Isolated Nginx (webserver) with Basic configuration for nginx server
  - Isolated PHP server that support fastcgi (fpm)
  - Isolated mysql service
  - Starter laravel project make connection with mysql database
  - Handle the services in docker-compose file


### Installation
###### `Here i use Ubuntu 18.4 As my operating system`
First install docker and docker compose in your machine
Validate if this already installed in your machine or not by this commands
```sh
$ sudo docker --version
$ sudo docker-compose --version
```
download the repo 
```sh
$ git clone https://github.com/hatem-elsheref/laravel-with-docker.git
$cd /../path/to/docker-compose.yaml
```
in the path of docker compose file 
```sh
$ sudo docker-compose build --no-cache
$ sudo docker-compose up
$ open the application dir in your ide
$ remove composer.lock file and run > sudo composer update
$ change the database connection connfigurations in .env file to
$ change the permissions of storage dir
$ generate new key > php artisan key:generate
$ run migrations file > php artisan migrate:fresh --seed

> DB_CONNECTION=mysql
> DB_HOST=mysql_server
> DB_PORT=3306
> DB_DATABASE=laravel
> DB_USERNAME=hatem
> DB_PASSWORD=webserver
```

License
----
MIT
