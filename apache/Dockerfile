FROM httpd:2.4
RUN apt-get update && apt-get upgrade
# Copy apache vhost file to proxy php requests to php-fpm container
COPY ./conf/default.conf /usr/local/apache2/conf/default.conf
RUN echo "Include /usr/local/apache2/conf/default.conf" \
    >> /usr/local/apache2/conf/httpd.conf