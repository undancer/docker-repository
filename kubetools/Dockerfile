FROM undancer/ubuntu

LABEL author="undancer, undancer@gmail.com"

RUN apt-get -qq update && \
    apt-get -y install \
    curl wget && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

RUN apt-get update && apt-get -y upgrade
RUN echo hello

CMD ["bash"]
