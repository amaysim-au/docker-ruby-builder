FROM ruby:2.7-slim

ENV GECKO_VERSION 0.32.0

# install build deps
RUN	echo "deb http://mozilla.debian.net/ jessie-backports firefox-esr" >> /etc/apt/sources.list && \
    apt-get update && \
    apt-get -y --force-yes -t jessie-backports install build-essential  \
    libpq-dev postgresql-client nodejs xvfb tzdata make git wget firefox-esr curl && \
    echo "StrictHostKeyChecking no" >> /etc/ssh/ssh_config

# install gecko driver
RUN wget https://github.com/mozilla/geckodriver/releases/download/v${GECKO_VERSION}/geckodriver-v${GECKO_VERSION}-linux64.tar.gz -O /tmp/geckodriver.tar.gz && \
    tar -C /usr/local/bin -xvzf /tmp/geckodriver.tar.gz && \
    rm /tmp/geckodriver.tar.gz

CMD [ "ruby", "-v" ]
