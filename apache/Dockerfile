FROM php:apache-bullseye

# Instalar los drivers de MySQLi
RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli

RUN apt-get update

RUN apt-get upgrade -y

RUN apt-get install curl -y

RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -

RUN apt-get install node.js -y

# Copiar los archivos del sitio web al directorio del sitio en el contenedor
COPY . /var/www/html/