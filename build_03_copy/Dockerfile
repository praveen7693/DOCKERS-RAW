FROM alpine:latest
LABEL Owner="pnatanas"
RUN apk add --update supervisor nginx && rm -rf /var/cache/apk/*
COPY start.sh /script/
COPY files/default.conf /etc/nginx/conf.d/
COPY files/nginx.conf /etc/nginx/nginx.conf
COPY files/supervisord.conf /etc/supervisor.conf