FROM nginx

# copy config file
COPY nginx.conf /etc/nginx/nginx.conf

# copy html content
COPY static /data/www/

# am Ende soll nginx ausgeführt werden
CMD ["nginx"]

EXPOSE 80
EXPOSE 443
