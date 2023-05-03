FROM wuzhenhua/base

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

RUN yum install -y --disablerepo=updates firefox wqy-microhei-fonts && yum clean all
RUN dbus-uuidgen >/var/lib/dbus/machine-id

CMD ["firefox"]
