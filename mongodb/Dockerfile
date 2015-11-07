FROM undancer/ubuntu
MAINTAINER undancer , undancer@gmail.com

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10 && \
    echo "deb http://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.0 multiverse" | tee /etc/apt/sources.list.d/mongodb-org-3.0.list && \
    apt-get -qq update && \
    apt-get -y install \
      mongodb-org \
      mongodb-org-mongos \
      mongodb-org-server \
      mongodb-org-shell \
      mongodb-org-tools \
    && \
    echo "mongodb-org hold"         | dpkg --set-selections && \
    echo "mongodb-org-server hold"  | dpkg --set-selections && \
    echo "mongodb-org-shell hold"   | dpkg --set-selections && \
    echo "mongodb-org-mongos hold"  | dpkg --set-selections && \
    echo "mongodb-org-tools hold"   | dpkg --set-selections && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

CMD ["bash"]
