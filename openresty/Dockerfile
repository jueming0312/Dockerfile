FROM openresty/openresty:1.19.9.1-alpine

RUN addgroup -g 500 www && adduser -G www -u 500 -D www \
&& mkdir /usr/local/openresty/nginx/conf/vhosts -p \
&& mkdir /data/wwwroot/ -p \
&& mkdir /data/wwwlogs/nginx/json/ -p \
&& chown www.www /data/wwwlogs/nginx/json

COPY nginx.conf /usr/local/openresty/nginx/conf/nginx.conf