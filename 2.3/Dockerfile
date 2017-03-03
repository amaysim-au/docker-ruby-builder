FROM ruby:2.3

RUN	apt-get update && \
	DEBIAN_FRONTEND=noninteractive && \
    apt-get -y install nodejs postgresql-client iceweasel xvfb phantomjs

CMD [ "ruby", "-v" ]
