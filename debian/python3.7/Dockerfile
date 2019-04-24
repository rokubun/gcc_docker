FROM python:3.7-slim-stretch

# Install some basic tools
RUN apt-get update && apt-get install -y \
        bash \
        gcc \    
        g++ \
        make \
        cmake \
        valgrind \
        binutils \
        tar \
        gzip \
        git \
        uncrustify \
        gdb \
        doxygen \
        graphviz \
    && rm -rf /var/lib/apt/lists/*
        

# Get yamlcpp and install it
ARG YAMLCPP_URL=https://github.com/jbeder/yaml-cpp.git
ARG YAMLCPP_TAG=yaml-cpp-0.6.2

RUN git clone --depth 1 --branch ${YAMLCPP_TAG} ${YAMLCPP_URL} \
    && (cd yaml-cpp; cmake -DCMAKE_INSTALL_PREFIX=${USRLOCAL} . ; make -j 8; make install) \
    && rm -rf yaml-cpp \
    && pip install -U pytest
