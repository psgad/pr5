FROM ubuntu:latest

RUN apt update \
    && apt upgrade \
    && apt install -y \x11-apps \
    xauth \
    && rm -rf /var/lib/apt/lists/*

ENV DISPLAY=host.docker.internal:0

CMD ["xeyes"]
    