FROM ubuntu:latest

MAINTAINER	erog38@gmail.com
VOLUME ["/opt/blog"] 
RUN apt-get update 
RUN apt-get install ca-certificates -y
RUN useradd -ms /bin/bash solo
RUN chown -R solo /opt/blog
WORKDIR /opt/blog
CMD ["/opt/blog/blog", "/opt/blog/config.json"]
