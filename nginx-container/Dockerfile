FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y nginx
RUN apt-get install openssh-server -y

RUN echo 'root:root' | chpasswd

ADD nginx.conf /etc/nginx/nginx.conf
ADD ./www /www
ADD sshd_config /etc/ssh/sshd_config

EXPOSE 80
CMD service ssh start && nginx