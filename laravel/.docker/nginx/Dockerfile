FROM nginx:1.13.5-alpine

COPY nginx.conf /etc/nginx/nginx.conf
COPY vhost.conf /etc/nginx/conf.d/default.conf

RUN addgroup --gid 3000 --system app
RUN adduser --uid 3000 --system --disabled-login --disabled-password --gid 3000 app

EXPOSE 80
EXPOSE 443

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]