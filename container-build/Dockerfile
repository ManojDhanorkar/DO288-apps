# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent
LABEL L1=OCP
LABEL L2=K8s
RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf
RUN chgrp -R 0 /var/log/httpd /var/run/httpd && chmod -R g=u /var/log/httpd /var/run/httpd 
USER 1001