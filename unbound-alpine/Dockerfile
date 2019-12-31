FROM alpine:3.11

RUN apk add unbound \
      && mkdir -p /etc/unbound/ \
      && wget -S https://www.internic.net/domain/named.cache -O /etc/unbound/root.hints

COPY ./unbound.conf /etc/unbound/unbound.conf 
