FROM ubuntu:20.04

WORKDIR /usr/src/app

COPY script.sh .

RUN apt-get -y update && apt-get -y install curl

RUN chmod +x script.sh

CMD ./script.sh
