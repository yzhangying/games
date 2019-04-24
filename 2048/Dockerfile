FROM centos


RUN yum install -y epel-release && yum install -y nginx 


RUN  mkdir -p /var/www/html/
ADD  html/   /var/www/html/

ADD nginx.conf /etc/nginx/nginx.conf

RUN chmod 644 /etc/nginx/nginx.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

