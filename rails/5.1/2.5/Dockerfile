FROM ruby:2.5-alpine

ENV RAILS_VERSION 5.1.4

RUN apk -U upgrade \
  && apk add -t build-dependencies \
  	build-base \
    postgresql-dev \
  && apk add \
    tzdata \
    nodejs \
    yarn \
  && rm -rf /tmp/* \
  && rm -rf /var/cache/apk/* 

RUN gem install rails -v "$RAILS_VERSION"

EXPOSE 3000 3035
