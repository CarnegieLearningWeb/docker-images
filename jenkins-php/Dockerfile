FROM php:7.4.7

# The mkdir command is a workaround for a bug when installing java on a debian slim image
# https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=863199
# Even though this container is for php, java needs to be installed for jenkins to connect to the container
RUN mkdir -p /usr/share/man/man1 && \
    apt update && \
    apt install -y openjdk-11-jre git

RUN curl -sS https://getcomposer.org/installer | php && \
    php composer.phar require pheromone/phpcs-security-audit && \
    sh vendor/pheromone/phpcs-security-audit/symlink.sh

ENV PATH="/vendor/bin:${PATH}"