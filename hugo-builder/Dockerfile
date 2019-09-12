FROM alpine:latest

MAINTAINER feffe <feffe@feffe.dev>

ENV VERSION 0.58.1
RUN apk add --no-cache git openssl py-pygments curl \
    && curl -L https://github.com/gohugoio/hugo/releases/download/v${VERSION}/hugo_extended_${VERSION}_Linux-64bit.tar.gz | tar -xz \
    && mv hugo /usr/bin/hugo \
    && apk del curl
