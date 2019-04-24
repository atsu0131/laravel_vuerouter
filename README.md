# Docker for Laravel and Vue development


## Get docker files
```
$ ls 

docker                  docker-compose.yml
```

## Docker run

```
$ docker-compose up -d --build
```

```
$ docker-compose ps
      Name                     Command              State                 Ports
---------------------------------------------------------------------------------------------
laravel-app_app_1   docker-php-entrypoint php-fpm   Up      9000/tcp
laravel-app_db_1    docker-entrypoint.sh mysqld     Up      0.0.0.0:3306->3306/tcp, 33060/tcp
laravel-app_web_1   nginx -g daemon off;            Up      0.0.0.0:80->80/tcp
```

## Make Laravel project

```
$ docker-compose exec app laravel new
```

## Access Laravel App

```
$ cp .env.example .env
```

## Use composer

```
$ docker-compose up -d
$ composer update
```

http://localhost

## Install Vue

 ```
 $ docker-compose exec app bash
  ```

Install node:
 ```
 # npm install
 ```
Build dev: 
```
 # npm run dev
```
Build production: 
```
 # npm run production
```
Watch: 
```
 # npm run watch
```

## Use migration

```
 $ docker-compose exec app bash

 # php artisan migrate
```