FROM ubuntu:latest
MAINTAINER u6k <u6k.apps@gmail.com>

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y build-essential git wget

RUN wget https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.0.tar.gz && \
    tar zxvf ruby-2.3.0.tar.gz && \
    cd ruby-2.3.0/ && \
    ./configure && \
    make && \
    make install

CMD [ "ruby", "-v" ]
