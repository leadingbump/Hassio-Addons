ARG BASE=mbentley/ubuntu:20.04
FROM ${BASE}

RUN sudo apt-get update -y
RUN sudo apt-get install -y python3
RUN sudo apt-get install -y pip3



COPY lc7001-mqtt-bridge.py lc7001-mqtt-bridge.conf run.sh

RUN a+x chmod /run.sh

CMD [ "/run.sh" ]
