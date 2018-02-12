FROM ubuntu:latest
MAINTAINER razu <razu@devspree.com>

RUN apt-get install -y redis-server

COPY redis.conf /etc/redis/

CMD ["redis-server", "/etc/redis/redis.conf"]