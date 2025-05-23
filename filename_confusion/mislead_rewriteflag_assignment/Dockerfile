FROM httpd:2.4.46
RUN apt-get update && apt-get install -y apache2-utils php-cgi
RUN mkdir -p /usr/local/apache2/cgi-bin && \
    echo '#!/bin/sh\nexec /usr/bin/php-cgi' > /usr/local/apache2/cgi-bin/php-cgi && \
    chmod +x /usr/local/apache2/cgi-bin/php-cgi