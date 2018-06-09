FROM 1132053388/base:jdk8-jce
MAINTAINER "sunfit.cn"

#时区设置
sed -i 's/Etc\/UTC/Asia\/Shanghai/' /etc/timezone

#配置tomcat
WORKDIR /root
COPY apache-tomcat-8.0.52.tar.gz .
RUN tar -zxvf apache-tomcat-8.0.52.tar.gz && mv apache-tomcat-8.0.52 tomcat-8.0.52
RUN rm -rf apache-tomcat-8.0.52.tar.gz


