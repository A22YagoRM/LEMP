FROM debian:latest

RUN apt update && apt install -y apache2 php libapache2-mod-php

RUN apt install -y php-zip php-xml php-curl php-gd php-mysql php-intl php-mbstring

RUN a2enmod ssl
RUN a2enmod rewrite

EXPOSE 80
EXPOSE 443

#CMD chmod 777 /app/prestashop/ && apachectl -D FOREGROUND
CMD apachectl -D FOREGROUND