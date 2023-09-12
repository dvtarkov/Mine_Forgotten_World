FROM ubuntu:20.04

WORKDIR /srv/www/minecraft-server/

RUN apt update

RUN apt install openjdk-17-jre-headless -y
RUN apt install openjdk-17-jdk-headless -y

EXPOSE 25565

COPY . /srv/www/minecraft-server/