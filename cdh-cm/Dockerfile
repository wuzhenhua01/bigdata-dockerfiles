FROM wuzhenhua/cdh-base

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

RUN yum install -y cloudera-manager-server && yum clean all

RUN systemctl enable cloudera-scm-server

WORKDIR /var/log/cloudera-scm-server

EXPOSE 7180
