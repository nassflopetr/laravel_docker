FROM php:7.4-fpm

WORKDIR /var/www/html

RUN apt-get update \
    && docker-php-ext-install pdo_mysql
