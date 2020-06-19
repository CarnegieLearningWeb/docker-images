# jenkins-php
An image to use with the [Jenkins Docker Plugin](https://wiki.jenkins.io/display/JENKINS/Docker+Plugin)
for running source code analysis on php projects

Comes with the PHP CodeSniffer utility installed

To configure in Jenkins, go to Manage Jenkins -> Manage Nodes and Clouds -> Configure Clouds. Under Docker Agent templates:
* Docker Image = carnegielearning/php:latest
* Remote File System Root = /root
* Connect method = Attach Docker Container
* User = root