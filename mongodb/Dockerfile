FROM ivarg/base
MAINTAINER Ivar Gaitan <ivar.gaitan@gmail.com>

RUN apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10
RUN echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | \
    tee /etc/apt/sources.list.d/mongodb.list

RUN apt-get update && apt-get install -y \
    mongodb-org

# Create the MongoDB data directory
RUN mkdir -p /data/db

EXPOSE 27017

ENTRYPOINT ["mongod"]


