FROM ruby:2.7-alpine

RUN	echo "@testing http://nl.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories && \
    apk --update --no-cache --upgrade add apk-tools build-base libxml2-dev libxslt-dev postgresql-dev nodejs xvfb tzdata bash openssh-client git && \
    touch /etc/ssh/ssh_config && \
    echo "StrictHostKeyChecking no" >> /etc/ssh/ssh_config

CMD [ "ruby", "-v" ]
