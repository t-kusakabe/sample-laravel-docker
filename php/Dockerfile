FROM php:7.3.5-fpm-alpine3.9
COPY php.ini /usr/local/etc/php/

# install composer
RUN cd /usr/bin && curl -s http://getcomposer.org/installer | php && ln -s /usr/bin/composer.phar /usr/bin/composer

RUN docker-php-ext-install pdo_mysql

WORKDIR /var/www
