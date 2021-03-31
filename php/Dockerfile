FROM php:7.4.4-apache
RUN apt-get update && \
  apt-get install -y libonig-dev libzip-dev git \
  && docker-php-ext-install pdo_mysql mysqli zip

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer
