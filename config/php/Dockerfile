FROM php:7.4.26-fpm

LABEL maintainer="Alvaro Fimpel <afimpel@afimpel.com>"

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get -y install --fix-missing curl git  zip unzip libxml2-dev libbz2-dev zlib1g-dev libsqlite3-dev libsqlite3-0 mariadb-client libcurl4-openssl-dev libssl-dev

RUN docker-php-ext-install intl
RUN docker-php-ext-install curl
RUN docker-php-ext-install mysqli pdo pdo_mysql
RUN docker-php-ext-install soap
RUN docker-php-ext-enable mysqli
RUN docker-php-ext-enable pdo
RUN docker-php-ext-enable pdo_mysql
RUN docker-php-ext-enable curl
RUN docker-php-ext-enable soap