FROM php:8.1.3-fpm-bullseye

RUN apt-get update
RUN apt-get install -y locales curl

RUN apt-get clean && rm -rf /var/lib/apt/lists/*

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN docker-php-ext-install pdo_mysql

EXPOSE 9000
CMD [ "php-fpm" ]