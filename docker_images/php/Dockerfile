FROM ubuntu:22.04

COPY ./sources.list /etc/apt/sources.list
RUN apt-get update -y

RUN DEBIAN_FRONTEND=noninteractive apt-get install php8.1 -y
RUN apt-get install php-fpm -y
RUN apt-get install php-mysql -y

RUN apt-get install vim -y
RUN apt install iputils-ping -y
RUN apt install net-tools -y
EXPOSE 9000
ENTRYPOINT ["php-fpm8.1","-F"]