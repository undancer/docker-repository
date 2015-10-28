FROM ubuntu:14.04
MAINTAINER undancer , undancer@gmail.com

RUN apt-get -qq update && \
    apt-get -y install \
    curl wget && \
    rm -rf /var/lib/apt/lists/*

CMD ["bash"]
