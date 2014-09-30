oracle-java
===========

This is my attempt at providing a Docker Image containing Oracle Java. It uses [phusion/baseimage](https://registry.hub.docker.com/u/phusion/baseimage/).

### Tags

The following tags are available:

* `latest` (default) Oracle 7 JDK
* `7` Oracle 7 JDK
* `8` Oracle 8 JDK

So you might run the following:

    docker run -it thijsschnitger/oracle-java:8 java -version

