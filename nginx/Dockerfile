FROM ubuntu

MAINTAINER Leonardo Sales <lsales@globosat.com.br>

RUN apt-get update

RUN apt-get install -y nginx vim git

ADD exemplo /etc/nginx/sites-enabled/default

EXPOSE 8080
