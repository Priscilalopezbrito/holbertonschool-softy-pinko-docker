# Latest nginx version
FROM nginx:latest

# Copy softy-pinko-front-end files
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy conf
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000
EXPOSE 9000