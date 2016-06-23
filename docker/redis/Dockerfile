FROM alpine:latest

MAINTAINER Philipp Gérard

RUN apk --update add redis && \
  rm -rf /var/cache/apk/*

VOLUME /data
WORKDIR /data

EXPOSE 6379

ENTRYPOINT ["redis-server"]