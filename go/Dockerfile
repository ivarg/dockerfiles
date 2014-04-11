FROM ivarg/base
MAINTAINER Ivar Gaitan <ivar.gaitan@gmail.com>

RUN apt-get install -y \
    bzr \
    git \
    curl

## This Go release: 1.2.1
RUN curl -s https://go.googlecode.com/files/go1.2.1.linux-amd64.tar.gz | \
    tar -v -C /usr/local/ -xz

ENV PATH  /usr/local/go/bin:/usr/local/bin:/usr/local/sbin:/usr/bin:/usr/sbin:/bin:/sbin
ENV GOPATH /go
ENV GOROOT /usr/local/go

