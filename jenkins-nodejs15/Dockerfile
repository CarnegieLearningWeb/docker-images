FROM node:15.7.0-alpine3.12

RUN adduser -D jenkins
RUN addgroup jenkins ping

RUN apk --no-cache -U add \
    git \
    openjdk8 \