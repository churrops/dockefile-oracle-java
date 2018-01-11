# docker build -t oracle-java8-centos7:8u151 .

FROM centos:centos7.4.1708

WORKDIR /tmp

RUN curl -C - -LR#OH "Cookie: oraclelicense=accept-securebackup-cookie" -k "http://download.oracle.com/otn-pub/java/jdk/8u151-b12/e758a0de34e24606bca991d704f6dcbf/jdk-8u151-linux-x64.rpm" && \
    yum install -y /tmp/jdk-8u151-linux-x64.rpm && \
    rm -f /tmp/jdk-8u151-linux-x64.rpm

ENV JAVA_HOME /usr/java/jdk1.8.0_151

CMD ["bash"]
