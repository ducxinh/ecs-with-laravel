# Laravel Docker


## Template 1
```bash
sudo docker compose -f docker-compose.1.yml up --build
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