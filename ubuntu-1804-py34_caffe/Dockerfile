FROM ubuntu-1804-py34:latest

ENV DEBIAN_FRONTEND noninteractive

# RUN apt-get update && apt-get install -y  gcc  make
		
RUN apt upgrade  -y





run apt-get -y install libprotobuf-dev libleveldb-dev libsnappy-dev libopencv-dev libhdf5-serial-dev protobuf-compiler  git libgflags-dev  autoconf


run apt-get install --no-install-recommends libboost-all-dev
apt-get install autoconf
apt-get install libtool
apt-get install libopenblas-dev
apt-get install liblmdb-dev

#CXX src/caffe/solver.cpp
#In file included from src/caffe/solver.cpp:9:0:
#./include/caffe/util/hdf5.hpp:7:10: fatal error: hdf5.h: No such file or directory
# #include "hdf5.h"

cd /
git clone https://github.com/google/glog.git
cd glog
./autogen.sh && ./configure && make && make install



run  git clone autoreconfhttps://github.com/KurtKramer/caffe.git
run pip3 install scikit-image protobuf





cd python
for req in $(cat requirements.txt); do pip3 install $req; done


cd /caffe
edit Makefile.config
==================================

Python-3.4.10
PYTHON_INCLUDE := /Python-3.4.10 \
                  /Python-3.4.10/dist-packages/numpy/core/include   
				  
				  
PYTHON_INCLUDE := /Python-3.4.10 \
                /Python-3.4.10/dist-packages/numpy/core/include	


PYTHON_LIBRARIES := boost_python3 python3.4m
PYTHON_INCLUDE := /Python-3.4.10/Include/ \
                /usr/local/lib/python3.4/site-packages/numpy/core/include				
======================================


make all