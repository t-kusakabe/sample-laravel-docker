FROM php:8.2.31-fpm-alpine3.22

COPY php.ini /usr/local/etc/php/
COPY --from=composer:2 /usr/bin/composer /usr/bin/composer

RUN docker-php-ext-install pdo_mysql

WORKDIR /var/www
