# Instalar dependencias do composer
docker exec -it setup-php composer install 

# Gerar APP_KEY
docker exec -it setup-php artisan key:generate 

# Rodar migrations
docker exec setup-php php artisan migrate   
