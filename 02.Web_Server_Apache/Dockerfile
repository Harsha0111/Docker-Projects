FROM httpd:2.4

# Set ServerName globally to suppress AH00558 warning
RUN echo "ServerName localhost" >> /usr/local/apache2/conf/httpd.conf

# Copy index.html to Apache document root
COPY index.html /usr/local/apache2/htdocs/

# Expose port 80 (default HTTP port) inside the container
EXPOSE 80

# Start Apache in the foreground
CMD ["httpd", "-D", "FOREGROUND"]
