FROM php:8.3-apache

RUN apt-get update && apt-get install -y \
  libpq-dev \
  && docker-php-ext-install pdo pdo_pgsql

WORKDIR /var/www/html

COPY . .

RUN chown -R www-data:www-data /var/www/html

EXPOSE 80
