FROM php:8.2-cli

RUN apt-get update && apt-get install -y git nano curl

ADD --chmod=0755 https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/
RUN install-php-extensions gd xdebug ctype curl dom filter hash iconv json libxml mbstring openssl SimpleXML exif fileinfo intl memcached zip zlib

WORKDIR /app/
RUN chown -R application:application /app/
