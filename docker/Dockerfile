FROM quay.io/fedora/fedora:30-x86_64
LABEL version=1.0
LABEL maintainer="Gowrishankar Muthukrishnan <gmuthukr@redhat.com>"

RUN yum install -y openvswitch python3-pip && \
    yum clean all
RUN pip3 install netcontrold
ENTRYPOINT ["/usr/local/bin/ncd_watch"]
