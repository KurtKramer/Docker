FROM ubuntu:18.04

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get install -y \
	    gcc  \
		make \
		build-essential \
		libssl-dev \
		zlib1g-dev \
		libbz2-dev \
		libsqlite3-dev \
		wget
		
		
RUN apt-get update && \
    apt-get install -y \
        libncurses5-dev \
        libreadline6-dev \
        libgdbm-dev \
        liblzma-dev \
        tk8.5-dev
		
RUN apt upgrade  -y

ADD https://www.python.org/ftp/python/3.4.9/Python-3.4.9.tgz  /
ADD Python-3.4.9.tgz  /

RUN cd /Python-3.4.9 && ./configure && make -j 2 && make install


