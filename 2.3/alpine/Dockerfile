FROM ruby:2.3-alpine

RUN	echo "@testing http://nl.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories
    apk --update add --no-cache --upgrade --virtual .alpine-deps apk-tools && \
    apk add --no-cache --virtual .build-deps build-base libxml2-dev libxslt-dev \
	postgresql-dev nodejs xvfb tzdata firefox@testing bash

CMD [ "ruby", "-v" ]