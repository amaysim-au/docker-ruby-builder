FROM ruby:2.3

RUN wget https://github.com/mozilla/geckodriver/releases/download/v0.11.1/geckodriver-v0.11.1-linux64.tar.gz -O /tmp/geckodriver.tar.gz && \
	tar -C /usr/local/bin -xvzf /tmp/geckodriver.tar.gz && \
	apt-get update && \
	DEBIAN_FRONTEND=noninteractive && \
    apt-get -y install nodejs postgresql-client chromium iceweasel xvfb 

CMD [ "ruby", "-v" ]