FROM centos:centos7
MAINTAINER benxjc

RUN mkdir /opt/jdk

WORKDIR /opt/jdk

ADD ./jdk-8u131-linux-x64.tar.gz /opt/jdk/

ENV JAVA_HOME /opt/jdk/jdk1.8.0_131
ENV PATH $JAVA_HOME/bin:$PATH
ENV CLASSPATH .:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar

COPY ./jce_policy-8/UnlimitedJCEPolicyJDK8  /opt/jdk/jdk1.8.0_131/jre/lib/security/
