FROM ruby:2.3-slim

# install build deps
RUN	echo "deb http://mozilla.debian.net/ jessie-backports firefox-release" >> /etc/apt/sources.list && \
    apt-get update && \
    apt-get -y --force-yes -t jessie-backports install nodejs postgresql-client xvfb make firefox

CMD [ "ruby", "-v" ]