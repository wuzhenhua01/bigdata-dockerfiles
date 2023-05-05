FROM wuzhenhua/base

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

RUN yum install -y --disablerepo=updates httpd && yum clean all

COPY _h5ai /var/www/html/

EXPOSE 80
CMD ["httpd", "-DFOREGROUND"]
