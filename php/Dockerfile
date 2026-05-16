FROM php:8.2.31-fpm-alpine3.22
COPY php.ini /usr/local/etc/php/

# install composer
RUN cd /usr/bin && curl -s http://getcomposer.org/installer | php && ln -s /usr/bin/composer.phar /usr/bin/composer

RUN docker-php-ext-install pdo_mysql

WORKDIR /var/www
