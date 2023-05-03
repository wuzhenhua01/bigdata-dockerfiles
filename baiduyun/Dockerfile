FROM centos:7.6.1810

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

ADD baidunetdisk-4.11.5.x86_64.rpm .
RUN yum install -y --disablerepo=updates baidunetdisk-4.11.5.x86_64.rpm && yum clean all && rm -rf baidunetdisk-4.11.5.x86_64.rpm
