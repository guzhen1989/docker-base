FROM  centos:7
MAINTAINER "sunfit.cn"
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai  /etc/localtime
RUN yum -y install kde-l10n-Chinese #安装中文支持
RUN localedef -c -f UTF-8 -i zh_CN zh_CN.utf8 #配置显示中文
ENV LC_ALL zh_CN.utf8 #设置环境变量
RUN yum update -y && \
yum install -y wget && \
yum install -y unzip