FROM centos:centos7
MAINTAINER Stephen K Conklin <stephen@thinkedg.com>

# update and clean
RUN yum update -y && \
    yum clean all

# install Packages
RUN yum install -y which && \
    yum install -y sudo  && \
    yum install -y rpm-build && \
    yum clean all


