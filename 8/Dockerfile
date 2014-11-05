FROM phusion/baseimage:0.9.15

MAINTAINER Thijs Schnitger <thijs.schnitger@trifork.nl>

ENV HOME /root

RUN /etc/my_init.d/00_regen_ssh_host_keys.sh

CMD ["/sbin/my_init"]

RUN add-apt-repository -y ppa:webupd8team/java \
 && apt-get update
RUN echo debconf shared/accepted-oracle-license-v1-1 select true | debconf-set-selections
RUN apt-get install -y oracle-java8-installer oracle-java8-set-default
RUN apt-get clean \
 && apt-get autoclean
