FROM debian:buster-slim as rcore_builder

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
        gdb \
        doxygen \
        graphviz \
        cppcheck \
        pylint \
        vim \
        libyaml-cpp-dev \
    && rm -rf /var/lib/apt/lists/*
    
