FROM ubuntu:latest

RUN apt-get update
RUN apt-get install git -y
RUN apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_4.x && apt-get install -y nodejs && apt-get install -y npm

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN git clone https://github.com/sgarcia-dev/nodejs-examples.git

WORKDIR /usr/src/app/nodejs-examples/learnyounode

CMD nodejs helloworld.js