FROM nginx:alpine

ARG conf

COPY ./nginx/conf/nginx.conf  /etc/nginx/nginx.conf

USER root
RUN chown -R nginx:nginx /var/cache/nginx

WORKDIR /usr/local/tomcat/bin
CMD ["nginx", "-g", "daemon off;"]
