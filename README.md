# docker-ruby-builder
ruby builder with extra dependencies to run Webdriver and DB tests:

- build essentials
- nodejs
- git
- xvfb
- postgresql dev and client
- make
- tzdata
- firefox 51.0
- geckodriver 0.15.0

## Usage

    docker run amaysim/ruby-builder:2.5-slim bundle exec rake db:test:prepare
    docker run amaysim/ruby-builder:2.5-slim bundle exec rake
