ARG BASE=mbentley/ubuntu:20.04
FROM ${BASE}

RUN apt-get update -y
RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN pip3 install tendo
RUN pip3 install paho-mqtt


COPY lc7001-mqtt-bridge.conf lc7001-mqtt-bridge.py run.sh /

RUN a+x chmod /run.sh

CMD [ "/run.sh" ]
