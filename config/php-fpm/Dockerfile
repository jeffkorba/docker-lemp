FROM php:fpm-alpine

# RUN apk --update --no-cache add $PHPIZE_DEPS linux-headers imagemagick imagemagick-dev
RUN apk --update --no-cache add $PHPIZE_DEPS linux-headers
RUN pecl install xdebug
RUN docker-php-ext-install mysqli
RUN docker-php-ext-enable mysqli xdebug