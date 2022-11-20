FROM php:fpm-alpine

RUN apk add pcre-dev imagemagick imagemagick-dev ${PHPIZE_DEPS} \
	&& pecl install xdebug \
	&& pecl install imagick \
	&& docker-php-ext-install mysqli \
	&& docker-php-ext-enable imagick mysqli xdebug