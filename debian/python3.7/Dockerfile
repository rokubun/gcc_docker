FROM python:3.7-slim-buster

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
    && rm -rf /var/lib/apt/lists/* \
    && pip install -U pytest twine
    
