FROM php:7.1-fpm

# remove default nginx config
RUN rm -rf /etc/nginx/conf.d/default.conf

# install magento packages dependencies
RUN apt-get update && apt-get install -y \
	curl \
	php5-curl \
	php5-mysql \
	php5-mcrypt \
	php5-xdebug \
	php-apc

# install composer
RUN curl -sS https://getcomposer.org/installer |  php -- --install-dir=/usr/local/bin --filename=composer
