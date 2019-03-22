FROM centos

RUN yum install -y epel-release && yum update -y
RUN rpm -Uvh https://mirror.webtatic.com/yum/el7/webtatic-release.rpm
RUN yum install -y nginx1w && yum install -y nginx1w-module-headers-more

ENTRYPOINT ["/usr/sbin/nginx","-g","daemon off;"]

EXPOSE 80
