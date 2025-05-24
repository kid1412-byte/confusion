FROM httpd:2.4.46
RUN apt-get update && apt-get install -y apache2-utils
COPY httpd.conf /usr/local/apache2/conf/httpd.conf
RUN mkdir -p /usr/share/libreoffice/help
COPY help.html /usr/share/libreoffice/help/help.html
COPY index.html /usr/share/libreoffice/help/xss/index.html