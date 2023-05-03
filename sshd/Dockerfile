FROM wuzhenhua/systemd

LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

RUN /bin/echo "root" | passwd --stdin root
RUN yum install -y openssh-server openssh-clients && yum clean all
RUN systemctl enable sshd
