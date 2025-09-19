FROM ubuntu:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

# 시스템 패키지 업데이트 및 필수 패키지 설치
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y gcc g++ python3 python3-pip software-properties-common

# Python 패키지 최신 버전으로 업그레이드
RUN pip install --upgrade --break-system-packages cryptography==42.0.4 setuptools==78.1.1

# 타임존 설정
RUN ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime
RUN echo "Asia/Seoul" > /etc/timezone