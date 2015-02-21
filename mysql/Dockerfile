FROM undancer/ubuntu
MAINTAINER undancer , undancer@gmail.com

RUN \
  apt-get update && \
  apt-get -y install \
          mysql-server-5.6 && \
  rm -rf /var/lib/apt/lists/*

VOLUME /var/lib/mysql

# CMD ["bash"]

EXPOSE 3306
CMD ["mysqld"]
