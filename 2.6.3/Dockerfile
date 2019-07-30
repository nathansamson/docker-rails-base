FROM ruby:2.6.3-stretch

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list


RUN apt-get update
RUN apt-get install -y nodejs ruby-all-dev yarn libjemalloc1
RUN apt-get install -y postgresql-client --no-install-recommends


RUN gem install nokogiri -v 1.10.3
RUN gem install pg -v 1.1.4
RUN gem install mini_racer -v 0.2.6
RUN gem install curb -v 0.9.10
RUN gem install sassc -v 2.0.1
RUN gem install sassc -v 1.12.1
RUN gem install bootsnap -v 1.4.4
RUN gem install mgspack -v 1.2.10
RUN gem install scrypt -v 3.0.6
RUN gem install ffi -v 1.11.1
RUN gem install puma -v 1.12.1
