## oceanhub_jekyll
FROM ubuntu:16.10

## PRE CONFIGURATION, optimization for docker-compose building
RUN mkdir /data
RUN mkdir /workdir

## INSTALL SECTION
RUN apt-get -qq update && apt-get -qqy upgrade

# Installing needed applications using package manager
RUN apt-get install -qqy \
  wget \
  ruby \
  ruby-dev \
  bash-completion

RUN apt-get -qq update

RUN apt-get install -qqy \
  vim \
  gcc \
  sudo

RUN apt-get install -qqy \
  make

RUN gem update --system
RUN gem install jekyll
RUN gem install liquid
RUN gem install jekyll bundler

## SUFFIX CONFIGURATION
WORKDIR /workdir

