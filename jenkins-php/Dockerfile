FROM php:7.4.7

# The mkdir command is a workaround for a bug when installing java on a debian slim image
# https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=863199
# Even though this container is for php, java needs to be installed for jenkins to connect to the container
RUN mkdir -p /usr/share/man/man1 && \
    apt update && \
    apt install -y openjdk-11-jre git
    
RUN pear install PHP_CodeSniffer-3.5.5
