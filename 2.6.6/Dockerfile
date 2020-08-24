FROM ruby:2.6.6-buster

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list


RUN apt-get update
RUN apt-get install -y nodejs yarn libjemalloc2
RUN apt-get install -y postgresql-client --no-install-recommends


RUN gem install msgpack:1.3.3 scrypt:3.0.7 ffi:1.13.1  json:2.3.1 bindex:0.8.1
RUN gem install nokogiri:1.10.10 pg:1.2.3 mini_racer:0.3.1 stackprof:0.2.15
RUN gem install bootsnap:1.4.7
RUN gem install unf_ext:0.0.7.7 nio4r:2.5.2 puma:4.3.5 websocket-driver:0.7.3
RUN gem install scout_apm:2.6.8 rgeo:2.1.1 rinku:2.0.6
RUN gem install sassc:2.4.0
