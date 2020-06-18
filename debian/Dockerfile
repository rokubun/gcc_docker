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
        uncrustify \
        gdb \
        doxygen \
        graphviz \
        cppcheck \
        pylint \
    && rm -rf /var/lib/apt/lists/*
    
