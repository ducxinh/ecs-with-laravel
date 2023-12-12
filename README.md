# Laravel Docker


## Template 1
```bash
sudo docker compose -f docker-compose.1.yml up --build
ggpull && sudo docker compose -f docker-compose.1.yml up --build --remove-orphans
```
```bash
sudo docker ps


# 
sudo docker exec -it ecs-with-laravel-web-1 bash
ls -la
composer install
php artisan migrate

sudo docker exec -it ecs-with-laravel-mysql-1 bash
```

## Template 2
```bash
sudo docker compose -f docker-compose.2.yml up --build
ggpull && sudo docker compose -f docker-compose.2.yml up --build --remove-orphans
```
```bash
sudo docker ps


# 
sudo docker exec -it ecs-with-laravel-web-1 bash
sudo docker exec -it ecs-with-laravel-webapp-1 bash
ls -la
composer install
php artisan migrate

sudo docker exec -it ecs-with-laravel-mysql-1 bash
ls -la 
# bin  boot  dev	etc  home  lib	lib32  lib64  libx32  lost+found  media  mnt  node_modules  opt  proc  root  run  sbin	snap  srv  sys	tmp  usr  var  vendor
```

## Template 3
```bash
sudo docker compose -f docker-compose.3.yml up --build

ggpull && sudo docker compose -f docker-compose.3.yml up --build --remove-orphans

sudo docker ps

sudo docker exec -it ecs-with-laravel-webapp-1 bash
ls -la
composer install
php artisan migrate

sudo docker exec -it ecs-with-laravel-mysql-1 bash
ls -la 
# bin  boot  dev	etc  home  lib	lib32  lib64  libx32  lost+found  media  mnt  node_modules  opt  proc  root  run  sbin	snap  srv  sys	tmp  usr  var  vendor
```