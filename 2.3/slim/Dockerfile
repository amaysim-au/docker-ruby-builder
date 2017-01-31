FROM ruby:2.3-slim

RUN	apt-get update && \
	DEBIAN_FRONTEND=noninteractive && \
    apt-get -y install nodejs postgresql-client iceweasel xvfb 

CMD [ "ruby", "-v" ]