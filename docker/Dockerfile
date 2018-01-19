FROM sbeliakou/centos:7.3
MAINTAINER Kanstantsin Shchura
RUN yum -y install nginx
#COPY nginx_conf/https.conf /etc/nginx/conf.d/.
EXPOSE 80
EXPOSE 443
CMD ["nginx", "-g", "daemon off;"]

