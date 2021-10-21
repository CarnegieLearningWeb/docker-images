FROM jenkins/inbound-agent:latest

USER root

RUN apt-get -y update && \
    apt-get -y install git python2 python3 python3-pip

USER jenkins