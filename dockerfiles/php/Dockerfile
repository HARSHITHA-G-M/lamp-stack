FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Kolkata

RUN apt-get update && \
    apt-get install -y tzdata && \
    apt-get install -y php libapache2-mod-php php-mysql && \
    apt-get clean

CMD ["apachectl", "-D", "FOREGROUND"]

