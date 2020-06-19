# jenkins-node-ubuntu
An image to use with the [Jenkins Docker Plugin](https://wiki.jenkins.io/display/JENKINS/Docker+Plugin)

It has a bunch of useful tools that a Jenkins job might take advantage of, such as:
* Git
* Maven
* Curl
* Java
* Mysql 5.7 client
* OpenSSH client

To configure in Jenkins, go to Manage Jenkins -> Manage Nodes and Clouds -> Configure Clouds. Under Docker Agent templates:
* Docker Image = carnegielearning/jenkins-node-ubuntu:latest
* Remote File System Root = /home/jenkins
* Connect method = Attach Docker Container
* User = jenkins