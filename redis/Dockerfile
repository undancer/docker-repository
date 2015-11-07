FROM ubuntu:14.04
MAINTAINER undancer , undancer@gmail.com

RUN apt-get -qq update && \
    apt-get -y install \
      redis-server \
      redis-tools \
    && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

CMD ["bash"]
