FROM ruby:2.6.3-stretch

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list


RUN apt-get update
RUN apt-get install -y nodejs ruby-all-dev yarn libjemalloc1
RUN apt-get install -y postgresql-client --no-install-recommends


RUN gem install msgpack:1.2.10 scrypt:3.0.6 ffi:1.11.1
RUN gem install nokogiri:1.10.3 pg:1.1.4 mini_racer:0.2.6 sassc:2.0.1
RUN gem install curb:0.9.10 bootsnap:1.4.4
RUN gem install sassc:1.12.1
RUN gem install puma:1.12.1
