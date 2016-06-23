FROM alpine:latest

MAINTAINER Philipp Gérard

RUN \
  apk --update add memcached wget && \
  wget --no-check-certificate -O /usr/local/bin/gosu https://github.com/tianon/gosu/releases/download/1.9/gosu-amd64 && \
  chmod +x /usr/local/bin/gosu && \
  rm -rf /var/cache/apk/*

EXPOSE 11211

ENTRYPOINT ["gosu", "memcached", "memcached"]