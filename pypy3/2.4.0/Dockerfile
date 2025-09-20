FROM cheesesand/judge-base:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

RUN apt-get install -y wget
RUN wget https://bitbucket.org/pypy/pypy/downloads/pypy3-2.4.0-linux64.tar.bz2
RUN tar -C /opt -xvf pypy3-2.4.0-linux64.tar.bz2
RUN mv /opt/pypy3-2.4.0-linux64/ /opt/pypy3
RUN rm pypy3-2.4.0-linux64.tar.bz2
RUN rm -rf /var/lib/apt/lists/*
