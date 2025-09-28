FROM ubuntu:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

RUN apt-get update && apt-get upgrade -y \
    && apt-get install -y curl

# isolate 키 및 소스 추가
RUN mkdir -p /etc/apt/keyrings
RUN curl -fsSL https://www.ucw.cz/isolate/debian/signing-key.asc | tee /etc/apt/keyrings/isolate.asc > /dev/null
RUN echo "deb [arch=amd64 signed-by=/etc/apt/keyrings/isolate.asc] http://www.ucw.cz/isolate/debian/ bookworm-isolate main" | tee /etc/apt/sources.list.d/isolate.list

# 시스템 패키지 업데이트 및 필수 패키지 설치
RUN apt-get update \
    && apt-get install -y gcc g++ python3 software-properties-common isolate \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# 타임존 설정
RUN ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime \
    && echo "Asia/Seoul" > /etc/timezone
