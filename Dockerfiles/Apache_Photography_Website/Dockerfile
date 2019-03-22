FROM centos:6.6
MAINTAINER rohith
RUN yum install httpd -y
RUN chkconfig httpd on
ADD Photography /var/www/html/Photography
EXPOSE 80
ENTRYPOINT ["/usr/sbin/httpd"]
CMD ["-D", "FOREGROUND"]
