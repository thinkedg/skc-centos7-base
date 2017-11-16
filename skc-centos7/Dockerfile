FROM centos:centos7
MAINTAINER Stephen K Conklin <stephen@thinkedg.com>

# update and clean
RUN yum update -y && \
    yum clean all

# install Packages
RUN yum install -y which && \
    yum install -y sudo  && \
    yum install -y rpm-build && \
    yum install -y emacs && \
    yum clean all

# install Python3
RUN yum install -y https://centos7.iuscommunity.org/ius-release.rpm && \
    yum update -y && \
    yum install -y python35u python35u-libs python35u-devel python35u-pip && \
    yum clean all

RUN ln -s /usr/bin/python3.5 /usr/bin/python3

# install ruby
RUN echo 'insecure' >> /root/.curlrc && \
    gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB && \
    \curl -sSL https://get.rvm.io | bash -s stable --ruby && \
    yum clean all





