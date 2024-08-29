#FROM nginxinc/nginx-unprivileged:latest

ARG conf

COPY ./nginx/conf/nginx.conf  /etc/nginx/nginx.conf

#USER root
USER nginx
#RUN chown -R nginx:nginx /var/cache/nginx

WORKDIR /usr/local/tomcat/bin
CMD ["nginx", "-g", "daemon off;"]
