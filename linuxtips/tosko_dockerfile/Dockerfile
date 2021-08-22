FROM debian

LABEL app='megazord'
ENV VERSION=1.0

RUN apt-get update && apt-get install -y stress && apt-get clean

CMD stress --cpu 1 --vm-bytes 64M --vm 1

