FROM  wuzhenhua/base
LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

COPY linuxqq_2.0.0-b2-1089_x86_64.rpm .
RUN yum install -y --disablerepo=updates linuxqq_2.0.0-b2-1089_x86_64.rpm && rm -f linuxqq_2.0.0-b2-1089_x86_64.rpm
