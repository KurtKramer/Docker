FROM ubuntu-1804-py34:latest

ENV DEBIAN_FRONTEND noninteractive

# RUN apt-get update && apt-get install -y  gcc  make
		
RUN apt upgrade  -y
open


run apt-get -y install libprotobuf-dev \
                       libleveldb-dev libsnappy-dev \
					   libopencv-dev \
					   libhdf5-serial-dev \
					   protobuf-compiler  \
					   git \
					   libgflags-dev  \
					   autoconf

run apt-get -y install --no-install-recommends libboost-all-dev
#   run apt-get -y install autoconf libtool libopenblas-dev liblmdb-dev



# run cd / && git clone https://github.com/google/glog.git  && cd glog && ./autogen.sh && ./configure && make && make install

#  run pip3 install scikit-image protobuf

#  run cd / && git clone https://github.com/KurtKramer/caffe.git

#  run cd /caffe/python && for req in $(cat requirements.txt); do pip3 install $req; done

export CPATH="/usr/include/hdf5/serial/"

#  run cd /caffe && cp Makefile.config.ubuntu.py34 Makefile.config && make all 