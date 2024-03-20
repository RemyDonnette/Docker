FROM php:8.2-fpm

# Installation de dépendances pour l'activation de modules nécéssaires
RUN apt update \
    && apt install -y zip libzip-dev libpng-dev libicu-dev libxml2-dev

# Installation des modules
RUN docker-php-ext-install mysqli pdo pdo_mysql gd zip intl xml

# Nettoyage du cache
RUN apt clean