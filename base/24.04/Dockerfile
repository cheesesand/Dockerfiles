FROM ubuntu:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

# 시스템 패키지 업데이트 및 필수 패키지 설치
RUN apt-get update && apt-get upgrade -y \
    && apt-get install -y gcc g++ python3 software-properties-common \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# 타임존 설정
RUN ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime \
    && echo "Asia/Seoul" > /etc/timezone
