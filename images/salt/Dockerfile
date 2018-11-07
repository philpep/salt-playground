FROM debian:stretch
RUN apt-get update && apt-get -y install salt-master systemd-sysv
RUN systemctl disable getty@tty1.service
CMD ["/sbin/init"]
