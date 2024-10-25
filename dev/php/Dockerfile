FROM php:8.1-fpm-alpine AS base


RUN apk update && apk add --no-cache bash

WORKDIR /var/www/html




RUN apk add --no-cache $PHPIZE_DEPS linux-headers \
    && pecl install xdebug \
    && docker-php-ext-enable xdebug \
    && apk del $PHPIZE_DEPS


