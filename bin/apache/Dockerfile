FROM httpd:2.4.41-alpine
RUN apk update
RUN apk upgrade
RUN apk add nano
COPY demo.apache.conf /usr/local/apache2/conf/demo.apache.conf
RUN echo "Include /usr/local/apache2/conf/demo.apache.conf" \
    >> /usr/local/apache2/conf/httpd.conf

WORKDIR /usr/local/apache2/conf