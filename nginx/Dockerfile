FROM centos

MAINTAINER techmaster.vn

RUN rpm -Uvh http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm

# Install base stuff.
RUN yum -y install nginx unzip
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

CMD /usr/sbin/nginx
# Define mountable directories.
VOLUME ["/etc/nginx/sites-enabled","/etc/nginx/conf.d", "/var/log/nginx", "/var/www/html"]

USER root

# Define working directory.

WORKDIR /etc/nginx

# Expose ports.
EXPOSE 80


RUN echo "Success"
