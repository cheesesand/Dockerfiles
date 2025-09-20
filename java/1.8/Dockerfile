FROM cheesesand/judge-base:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

#RUN add-apt-repository -y ppa:webupd8team/java
RUN apt-get update
#RUN echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections
#RUN apt-get install -y oracle-java8-installer
RUN apt-get -y install openjdk-8-jdk
RUN rm -rf /var/lib/apt/lists/*
#RUN rm -rf /var/cache/oracle-jdk8-installer

#ENV JAVA_HOME /usr/lib/jvm/java-8-oracle
