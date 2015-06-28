FROM ruby:2.1.2

RUN bundle config --global frozen 1

RUN mkdir -p /usr/src/app

ADD . /usr/src/app/
WORKDIR /usr/src/app

RUN bundle install
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*