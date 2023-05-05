FROM wuzhenhua/sshd

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

COPY cloudera-manager.repo /etc/yum.repos.d/

COPY krb5.conf /etc/
RUN yum install -y krb5-workstation && yum clean all
