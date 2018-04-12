FROM ubuntu:latest

MAINTAINER	erog38@gmail.com
VOLUME ["/opt/Enterprise"] 
RUN apt-get update 
RUN apt-get install ca-certificates -y
RUN useradd -ms /bin/bash picard
RUN chown -R picard /opt/Enterprise
WORKDIR /opt/Enterprise
CMD ["/opt/Enterprise/Enterprise", "/opt/Enterprise/goicy.ini"]
