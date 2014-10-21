FROM ubuntu:14.04
MAINTAINER akshshar 

RUN echo "deb http://repos.mesosphere.io/ubuntu/ trusty main" > /etc/apt/sources.list.d/mesosphere.list
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv E56151BF
RUN apt-get -y update
RUN apt-get -y install wget unzip supervisor python mesos marathon 
