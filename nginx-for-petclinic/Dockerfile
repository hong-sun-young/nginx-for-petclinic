FROM nginx:latest

ARG conf

COPY ./nginx/conf/nginx.conf  /etc/nginx/nginx.conf

RUN mkdir -p /var/cache/nginx/client_temp && \
    chown -R nginx:nginx /var/cache/nginx

WORKDIR /usr/local/tomcat/bin
CMD ["nginx", "-g", "daemon off;"]
