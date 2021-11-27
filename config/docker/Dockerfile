FROM gabrielpcruz/npf:php73
ARG DEBIAN_FRONTEND=noninteractive

COPY nginx/sites-enabled/default /etc/nginx/sites-available/default
COPY nginx/fastcgi-php.conf /etc/nginx/snippets/fastcgi-php.conf
COPY php/php.ini /etc/php/7.3/fpm/php.ini

RUN apt-get update -y && apt-get install php7.3-soap -y