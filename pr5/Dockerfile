FROM ubuntu:latest

RUN apt update \
    && apt upgrade \
    && apt install -y \x11-apps \
    xauth \
    openjdk-17-jre \
    && rm -rf /var/lib/apt/lists/*

ENV DISPLAY=host.docker.internal:0

COPY calc.jar .

CMD ["java", "-jar", "calc.jar"]
    