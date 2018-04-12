FROM centos:7

MAINTAINER	dvd.red@gmail.com
COPY ./sc_serv.conf /etc/sc_serv.conf
RUN mkdir /opt/shoutserver
RUN curl http://download.nullsoft.com/shoutcast/tools/sc_serv2_linux_x64-latest.tar.gz | tar -xzC /opt/shoutserver/
WORKDIR /opt/shoutserver
CMD ["/usr/sbin/setcap", "CAP_NET_BIND_SERVICE=+eip", "/opt/shoutserver/sc_serv"] 
CMD ["/opt/shoutserver/sc_serv", "/etc/sc_serv.conf"]
