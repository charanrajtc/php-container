FROM php:fpm-alpine

RUN apk update && apk add  --no-cache $PHPIZE_DEPS
RUN docker-php-ext-install pdo_mysql 
RUN pecl install xdebug
COPY 99-xdebug.ini /usr/local/etc/php/conf.d/

CMD ["php-fpm","-F"]

EXPOSE 9000 9009