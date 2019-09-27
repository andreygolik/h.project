FROM nginx

ADD https://raw.githubusercontent.com/certbot/certbot/master/certbot-nginx/certbot_nginx/tls_configs/options-ssl-nginx.conf /etc/letsencrypt/conf/
ADD https://raw.githubusercontent.com/certbot/certbot/master/certbot/ssl-dhparams.pem /etc/letsencrypt/conf/
COPY ./dummy_certs/*.pem /etc/letsencrypt/live/default/

COPY ./conf.d/ /etc/nginx/conf.d/
