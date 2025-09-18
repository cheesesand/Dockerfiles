FROM ubuntu:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y gcc g++ python3
RUN apt-get install -y software-properties-common

RUN ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime
RUN echo "Asia/Seoul" > /etc/timezone
