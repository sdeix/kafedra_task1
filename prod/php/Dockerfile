FROM php:8.1-fpm-alpine AS base


RUN apk update && apk add --no-cache bash

WORKDIR /var/www/html

COPY index.php .

RUN apk add --no-cache curl \
    && docker-php-ext-install pdo pdo_mysql