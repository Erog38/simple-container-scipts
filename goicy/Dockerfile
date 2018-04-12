FROM ubuntu:latest

MAINTAINER	erog38@gmail.com
VOLUME ["/opt/goicy"] 
RUN useradd -ms /bin/bash goicy
RUN chown -R goicy /opt/goicy
WORKDIR /opt/goicy
CMD ["/opt/goicy/goicy", "/opt/goicy/goicy.ini"]
