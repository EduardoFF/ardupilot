FROM ubuntu:14.04
MAINTAINER Eduardo Feo Flushing <eduardo@idsia.ch>
LABEL Description="This image is used to crosscompile ArduCopter" Vendor="IDSIA" Version="1.0"


RUN apt-get update && apt-get install -y \
build-essential \
python-dev \
pkg-config-arm-linux-gnueabihf \
gawk \
g++-arm-linux-gnueabihf \
python-pip && rm -rf /var/lib/apt/lists/*

RUN pip install future

WORKDIR /root
USER root


VOLUME /ardupilot