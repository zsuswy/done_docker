FROM ubuntu:22.04

COPY ./sources.list /etc/apt/sources.list
RUN apt-get update -y

RUN apt-get install nginx -y

RUN apt-get install vim -y
RUN apt install iputils-ping -y
RUN apt install net-tools -y
EXPOSE 80
ENTRYPOINT ["nginx","-g","daemon off;"]