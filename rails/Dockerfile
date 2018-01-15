FROM ruby:2.5.0-alpine3.7

ENV RAILS_VERSION 5.1.4

RUN apk -U upgrade
RUN apk add build-base \
    postgresql-dev \
    tzdata \
    nodejs \
    yarn
RUN rm -rf /tmp/*
RUN rm -rf /var/cache/apk/*

RUN gem install rails -v "$RAILS_VERSION"

EXPOSE 3000 3035
