FROM nginx:1.15.0

RUN apt-get update

RUN apt-get install -y nginx

ADD index.html /usr/share/nginx/html/

RUN ln -sf /dev/stdout /var/log/nginx/access.log

RUN ln -sf /dev/stderr /var/log/nginx/error.log

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

