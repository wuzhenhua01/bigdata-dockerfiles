FROM  netherworld/systemd
LABEL maintainer="cx330.1000ly@gmail.com"
LABEL version="1.0.0"
LABEL description=""

RUN yum install -y krb5-server && yum clean all
RUN systemctl enable krb5kdc

COPY kdc.conf  /var/kerberos/krb5kdc/
COPY kadm5.acl /var/kerberos/krb5kdc/
COPY krb5.conf /etc/

RUN echo -e '\n' | kdb5_util create

EXPOSE 8464/tcp 8749/tcp 8888/tcp