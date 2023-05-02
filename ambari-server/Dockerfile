FROM  wuzhenhua/ambari-base

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

RUN yum install -y ambari-server mariadb --disablerepo=updates && yum clean all

RUN ambari-server setup \
  -j /usr/local/jdk \
  --database=mysql \
  --databasehost=wuzhenhua.cn \
  --databaseport=3306 \
  --databasename=ambari \
  --databaseusername=ambari \
  --databasepassword=ambari \
  -v \
  -s

RUN ambari-server install-mpack \
  --mpack=http://wuzhenhua.cn/HDF/centos7/3.x/updates/3.5.2.0/tars/hdf_ambari_mp/hdf-ambari-mpack-3.5.2.0-99.tar.gz \
  -v \
  -s

RUN systemctl enable ambari-server
RUN mysql -hwuzhenhua.cn -uambari -pambari ambari </var/lib/ambari-server/resources/Ambari-DDL-MySQL-CREATE.sql

WORKDIR /var/log/ambari-server

EXPOSE 8080
