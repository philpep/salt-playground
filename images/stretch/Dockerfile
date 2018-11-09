FROM debian:stretch
RUN apt-get update && apt-get -y install wget gnupg && \
    wget -O - https://repo.saltstack.com/apt/debian/9/amd64/2018.3/SALTSTACK-GPG-KEY.pub | apt-key add - && \
    echo "deb http://repo.saltstack.com/apt/debian/9/amd64/2018.3 stretch main" > /etc/apt/sources.list.d/saltstack.list && \
    apt-get update && apt-get -y install salt-minion systemd-sysv
RUN systemctl disable getty@tty1.service
CMD ["/sbin/init"]
