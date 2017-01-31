FROM ruby:2.3-alpine

RUN	apk --update add --no-cache --upgrade --virtual .alpine-deps apk-tools && \
    apk add --no-cache --virtual .build-deps build-base libxml2-dev libxslt-dev \
	postgresql-dev nodejs xvfb

RUN apk add --no-cache firefox-esr bash

CMD [ "ruby", "-v" ]