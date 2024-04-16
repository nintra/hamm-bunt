FROM php:8.2-fpm-alpine
# RUN apt-get update && apt-get install -y git nano curl
RUN apk update && apk add --no-cache libxml2-dev nano git curl

RUN curl -sSL https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions -o - | sh -s \
    gd xdebug ctype curl dom filter hash iconv json libxml mbstring openssl SimpleXML exif fileinfo intl memcached zip zlib

WORKDIR /var/www/html/
