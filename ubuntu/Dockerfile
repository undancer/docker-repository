FROM ubuntu:22.10

LABEL author="undancer, undancer@gmail.com"

RUN apt-get -qq update && \
    apt-get -y install \
    curl wget && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

CMD ["bash"]
