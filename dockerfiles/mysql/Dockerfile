FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Kolkata

RUN apt-get update && \
    apt-get install -y tzdata && \
    DEBIAN_FRONTEND=noninteractive apt-get install -y mysql-server && \
    apt-get clean

CMD ["mysqld_safe"]

