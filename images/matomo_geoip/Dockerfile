FROM bitnami/matomo:3.4.0

RUN apt-get update
RUN apt-get install -y php5-geoip php5-dev libgeoip-dev
RUN pecl channel-update pecl.php.net
RUN pecl install geoip-1.1.1

RUN echo "extension=geoip.so\ngeoip.custom_directory=/bitnami/matomo" > tempfile
RUN cat /opt/bitnami/php/etc/php.ini tempfile > temp.ini
RUN sudo mv temp.ini /opt/bitnami/php/etc/php.ini
RUN rm tempfile

EXPOSE 80 443

ENTRYPOINT ["/app-entrypoint.sh"]
CMD ["nami","start","--foreground","apache"]
