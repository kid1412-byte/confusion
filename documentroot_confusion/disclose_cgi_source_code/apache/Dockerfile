FROM httpd:2.4.46
RUN apt-get update && \
    apt-get install -y perl && \
    mkdir -p /usr/lib/cgi-bin
COPY download.cgi /usr/lib/cgi-bin/download.cgi
COPY httpd.conf /usr/local/apache2/conf/httpd.conf
RUN chmod +x /usr/lib/cgi-bin/download.cgi
