FROM php:8.2-fpm

RUN sed -i 's|^;access.log =.*|access.log = /proc/self/fd/2|' /usr/local/etc/php-fpm.d/www.conf && \
    echo "request_slowlog_timeout = 5s" >> /usr/local/etc/php-fpm.d/www.conf && \
    echo "slowlog = /proc/self/fd/2" >> /usr/local/etc/php-fpm.d/www.conf && \
    echo "php_admin_value[error_log] = /proc/self/fd/2" >> /usr/local/etc/php-fpm.d/www.conf && \
    echo "php_admin_flag[log_errors] = on" >> /usr/local/etc/php-fpm.d/www.conf