FROM php:8.1.5RC1-fpm-alpine3.15

COPY --from=composer:2.3.5 /usr/bin/composer /usr/bin/composer

RUN apk add --no-cache zip unzip libpq-dev

RUN docker-php-ext-install pdo pdo_mysql opcache
