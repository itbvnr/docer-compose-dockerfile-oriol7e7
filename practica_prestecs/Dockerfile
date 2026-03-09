FROM php:8.2-apache
#actualitzacions
RUN sudo apt update
RUN sudo apt upgrade

#instalacio mysqli
RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli

#activar mod d'apache i permisos usuari apache al director /var/www/html
RUN a2enmod rewrite
RUN chown -R www-data:www-data /var/www/html