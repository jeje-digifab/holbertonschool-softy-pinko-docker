FROM nginx:latest

RUN apt-get update && apt-get upgrade -y

RUN mkdir -p /var/www/html/softy-pinko-front-end

COPY ./proxy.conf /etc/nginx/conf.d/default.conf
