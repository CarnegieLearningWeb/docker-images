FROM alpine:3.12.0

RUN adduser -D jenkins
RUN addgroup jenkins ping

RUN apk --no-cache -U add \
    aws-cli \
    curl \
    git \
    jq \
    nodejs \
    npm \
    openjdk8 \
    wget \
    zip

ENV TERRAFORM_VERSION 0.13.0

RUN wget https://releases.hashicorp.com/terraform/${TERRAFORM_VERSION}/terraform_${TERRAFORM_VERSION}_linux_amd64.zip \
    && unzip terraform*.zip \
    && mv terraform /usr/local/bin