# Dockerfile von n1
FROM nginx


# zum Debugging
RUN apt-get update
RUN apt-get install -y curl


# copy config file
COPY nginx.conf /etc/nginx/nginx.conf


# copy html content
COPY static /data/www/


# don't daemonize
RUN echo "daemon off;" >> /etc/nginx/nginx.conf

# der hier sollte zur nginx.conf passen...
EXPOSE 80

# am Ende soll nginx ausgeführt werden
CMD service nginx start
