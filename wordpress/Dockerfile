FROM wordpress:6.8.2-php8.3-fpm

LABEL maintainer="Your Name"
LABEL project="WordPress Docker Compose"

RUN apt-get update && \
    apt-get install -y \
        curl \
        unzip \
        nano \
    && rm -rf /var/lib/apt/lists/*

COPY php.ini /usr/local/etc/php/conf.d/custom.ini

WORKDIR /var/www/html

EXPOSE 9000

CMD ["php-fpm"]
