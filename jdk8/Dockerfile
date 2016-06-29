FROM centos:latest
MAINTAINER Edgard Leal <edgardleal@gmail.com>

RUN yum -y update && yum -y install  wget unzip && yum clean all

RUN wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie"  http://download.oracle.com/otn-pub/java/jdk/8u40-b25/jdk-8u40-linux-x64.rpm && \
yum -y install jdk-8u40-linux-x64.rpm && \
rm jdk-8u40-linux-x64.rpm &&  yum clean all

RUN ["java","-version"]
CMD /bin/bash
