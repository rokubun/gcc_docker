FROM alpine:edge as rcore_builder

# Install some basic tools
RUN apk --no-cache add \
        bash \
        build-base \
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
        graphviz 