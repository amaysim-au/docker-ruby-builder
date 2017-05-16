FROM ruby:2.4

RUN	apt-get update && \
	DEBIAN_FRONTEND=noninteractive && \
    apt-get -y install nodejs postgresql-client iceweasel xvfb && \
    echo "StrictHostKeyChecking no" >> /etc/ssh/ssh_config

CMD [ "ruby", "-v" ]
