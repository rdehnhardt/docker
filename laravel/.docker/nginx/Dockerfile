FROM nginx:1.13.5-alpine

COPY nginx.conf /etc/nginx/nginx.conf
COPY vhost.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
EXPOSE 443

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]