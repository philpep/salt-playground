FROM centos:7
RUN yum -y install https://repo.saltstack.com/yum/redhat/salt-repo-latest-2.el7.noarch.rpm && \
    yum clean expire-cache && \
    yum -y install salt-minion
RUN systemctl enable salt-minion.service
RUN systemctl disable getty@tty1.service
CMD ["/usr/sbin/init"]
