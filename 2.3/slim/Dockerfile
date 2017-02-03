FROM ruby:2.3-slim

# install build deps
RUN	echo "deb http://mozilla.debian.net/ jessie-backports firefox-release" >> /etc/apt/sources.list && \
    apt-get update && \
    apt-get -y --force-yes -t jessie-backports install build-essential  \
    libpq-dev postgresql-client nodejs xvfb tzdata make git firefox

CMD [ "ruby", "-v" ]