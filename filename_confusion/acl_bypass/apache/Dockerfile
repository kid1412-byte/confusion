FROM httpd:2.4.46
RUN apt-get update && apt-get install -y apache2-utils
COPY .htpasswd /usr/local/apache2/.htpasswd
COPY httpd.conf /usr/local/apache2/conf/httpd.conf
