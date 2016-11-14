FROM nginx:1.11-alpine
RUN apk add --no-cache openssl && \
      openssl dhparam -out /etc/ssl/certs/dhparam.pem 4096 && \
      apk del --no-cache openssl
COPY config/ /etc/nginx/conf.d/