FROM ubuntu:16.04

RUN apt-get -y update

RUN  apt-get install -y  \
  gcc \
  make \
  git  \
  wget \
  build-essential \
  devscripts \
  fakeroot \
  debhelper \
  libsystemd-dev


RUN wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb
RUN dpkg -i erlang-solutions_1.0_all.deb
RUN apt-get update -y
RUN apt-get install erlang=1:21.0-1 -y
RUN apt-get install -y erlang-dev \
                       erlang-eunit
