FROM undancer/centos
MAINTAINER undancer , undancer@gmail.com

RUN curl -C -j -k -L \
    -H "Cookie: oraclelicense=accept-securebackup-cookie" \
    -o "jdk-linux-x64.rpm" \
    "http://download.oracle.com/otn-pub/java/jdk/7u75-b13/jdk-7u75-linux-x64.rpm" && \
    yum install -y jdk-linux-x64.rpm && \
    rm -f jdk-linux-x64.rpm

CMD ["bash"]
