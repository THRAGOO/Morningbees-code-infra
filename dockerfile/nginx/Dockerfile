FROM nginx:1.11
MAINTAINER jeong.minkyo <jeong.minkyo13@gmail.com>
 
RUN rm -rf /etc/nginx/conf.d/default.conf
 
COPY conf/morningbees-api.conf  /etc/nginx/conf.d/morningbees-api.conf
COPY conf/nginx.conf  /etc/nginx/nginx.conf
 
VOLUME ["/data", "/etc/nginx", "/var/log/nginx"]
 
WORKDIR /etc/nginx
 
CMD ["nginx"]
 
EXPOSE 80
EXPOSE 443

