FROM debian:bookworm

ARG DEBIAN_FRONTEND=noninteractive

RUN apt update && \
apt install -y \
tzdata \
goaccess && \
apt clean

VOLUME /srv/report

CMD ["goaccess", "--no-global-config", "--config-file=/srv/data/goaccess.conf"]