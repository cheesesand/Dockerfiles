FROM cheesesand/judge-base:24.04
MAINTAINER cheesesand <choijoung1479@gmail.com>

RUN apt-get update && apt-get install -y git build-essential
RUN git clone https://github.com/rdebath/Brainfuck.git /tmp/Brainfuck
RUN cd /tmp/Brainfuck && make
run cp /tmp/Brainfuck/bin/bf /usr/local/bin/
RUN cd / && rm -rf /tmp/Brainfuck

RUN rm -rf /var/lib/apt/lists/*
