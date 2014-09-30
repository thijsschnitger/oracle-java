FROM phusion/baseimage
MAINTAINER Thijs Schnitger <thijs.schnitger@trifork.nl>

RUN add-apt-repository -y ppa:webupd8team/java \
 && apt-get update \
 && echo debconf shared/accepted-oracle-license-v1-1 select true | debconf-set-selections \
 && apt-get install -y oracle-java8-installer oracle-java8-set-default \
 && apt-get clean \
 && apt-get autoclean
