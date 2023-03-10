FROM php:8-fpm
RUN apt-get update && \
    apt-get install -y \
      libzip-dev \
      zip \
      unzip \
      && docker-php-ext-install pdo_mysql \
      && docker-php-ext-install zip \
      && docker-php-ext-enable zip

WORKDIR /var/www/html
EXPOSE 9000
