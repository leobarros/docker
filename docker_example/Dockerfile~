FROM ubuntu

MAINTAINER Leonardo Sales <lsales@globosat.com.br>

RUN apt-get update

RUN apt-get install -y nginx vim git

ADD exemplo /etc/nginx/sites-enabled/default

RUN echo "daemon off;" >> /etc/nginx/nginx.conf

ADD ./ /rails

WORKDIR /rails

EXPOSE 8080

#trocando para entrypoint
#CMD service nginx start

ENTRYPINT ["/usr/sbin/nginx"]
ENTRYPOINT ["/etc/init.d/nginx"]

CMD["start"]

