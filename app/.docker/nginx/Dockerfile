ARG NGINX_VERSION=1.17

FROM nginx:${NGINX_VERSION}-alpine

COPY ./.docker/nginx/default.conf /etc/nginx/conf.d/default.conf

WORKDIR /var/www/symfony/public

COPY ./public  ./
RUN chmod 775 /var/www/symfony/public