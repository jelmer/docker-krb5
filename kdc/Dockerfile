FROM debian:sid-slim
LABEL maintainer="jelmer@jelmer.uk"
RUN apt-get update && \
    apt-get -y install krb5-kdc && \
    apt-get clean
VOLUME /var/lib/krb5kdc
EXPOSE 88
ENTRYPOINT /usr/sbin/krb5kdc
