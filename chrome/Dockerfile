FROM  wuzhenhua/base
LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

COPY google-chrome-stable_current_x86_64.rpm .
RUN yum install -y --disablerepo=updates google-chrome-stable_current_x86_64.rpm wqy-microhei-fonts && rm -f google-chrome-stable_current_x86_64.rpm
