# Image
FROM nginx:latest

# Configuration files
ADD vhost.conf /etc/nginx/conf.d/default.conf
ADD nginx.conf /etc/nginx/nginx.conf

# Expose ports.
EXPOSE 80
EXPOSE 443

# Execute command
CMD ["nginx"]