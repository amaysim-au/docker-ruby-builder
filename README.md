# docker-ruby-builder
ruby builder with extra dependencies to run Webdriver and DB tests:

- nodejs
- git
- xvfb
- postgresql-client
- make
- firefox 51.0

## Usage

    docker run amaysim/ruby-builder:2.3-slim bundle exec rake db:test:prepare
    docker run amaysim/ruby-builder:2.3-slim bundle exec rake