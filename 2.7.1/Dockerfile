FROM ruby:2.7.1-buster

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list

RUN apt-get update
RUN apt-get install -y nodejs yarn libjemalloc2
RUN apt-get install -y postgresql-client --no-install-recommends

RUN gem install msgpack:1.3.3 bindex:0.8.1 scrypt:3.0.7 bcrypt:3.1.13 ffi:1.12.2
RUN gem install nokogiri:1.10.9 pg:1.2.3 mini_racer:0.2.9 sassc:2.3.0
RUN gem install byebug:11.1.2 bootsnap:1.4.6 websocket-driver:0.7.1
RUN gem install jaro_winkler:1.5.4 nio4r:2.5.2 puma:4.3.3
