FROM jenkins/inbound-agent:alpine
USER root
RUN apk --allow-untrusted --no-cache -U add \
    bash \
    curl \
    docker \
    git \
    maven \
    nodejs \
    npm \
    openjdk8 \
    openssh-client \
    mysql-client \
    perl \
    py-pip \
    python2 \
    python3 \
    grep
RUN pip3 install awscli
USER jenkins