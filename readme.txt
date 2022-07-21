https://www.digitalocean.com/community/tutorials/how-to-set-up-laravel-nginx-and-mysql-with-docker-compose


# Composer install inside docker
docker run --rm -v $(pwd):/app composer install


# Docker compose
docker-compose down -v && docker-compose up -d


# docker run command inside container
docker-compose exec <container_name> <command>
docker-compose exec app php artisan migrate
docker-compose exec app php artisan view:clear
docker-compose exec app php artisan config:clear
docker-compose exec app php artisan cache:clear
