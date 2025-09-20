FROM cheesesand/judge-base:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

RUN apt-get update
RUN apt-get install -y wget bzip2
RUN wget https://downloads.python.org/pypy/pypy3.10-v7.3.17-linux64.tar.bz2
RUN tar -C /opt -xvf pypy3.10-v7.3.17-linux64.tar.bz2
RUN mv /opt/pypy3.10-v7.3.17-linux64/ /opt/pypy3
RUN rm pypy3.10-v7.3.17-linux64.tar.bz2
RUN rm -rf /var/lib/apt/lists/*

ENV PATH="/opt/pypy3/bin:${PATH}"