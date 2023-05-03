FROM wuzhenhua/sshd

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

COPY ambari.repo  /etc/yum.repos.d/
COPY hdp.gpl.repo /etc/yum.repos.d/

WORKDIR /usr/local
ADD jdk-8u202-linux-x64.tar.gz .
RUN ln -s jdk1.8.0_202 jdk
ENV JAVA_HOME /usr/local/jdk
ENV PATH      $JAVA_HOME/bin:$PATH

WORKDIR /usr/share/java
ADD mysql-connector-java-5.1.38.jar .
RUN ln -s mysql-connector-java-5.1.38.jar mysql-connector-java.jar

COPY krb5.conf /etc/
RUN yum install -y krb5-workstation && yum clean all
