FROM  centos:7
MAINTAINER "sunfit.cn"
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai  /etc/localtime
RUN yum -y install kde-l10n-Chinese
RUN localedef -c -f UTF-8 -i zh_CN zh_CN.utf8
ENV LC_ALL zh_CN.utf8
RUN yum update -y && \
yum install -y wget && \
yum install -y unzip