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
		
RUN apt upgrade  -y

ADD Python-3.4.9.tgz  /

WORKDIR /Python-3.4.9

##CMD ./configure
##RUN make -j 4
##RUN make install
