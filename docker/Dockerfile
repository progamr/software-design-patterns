FROM php:7.4-cli
RUN apt update
RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
RUN php composer-setup.php
RUN php -r "unlink('composer-setup.php');"
RUN mv composer.phar /usr/local/bin/composer
WORKDIR /usr/src/myapp
# to go to a terminal on the image : `docker run --rm -it swdp /bin/bash`

