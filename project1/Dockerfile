FROM ubuntu/apache2 

WORKDIR /app

COPY . /app

# Copy the Apache configuration file
COPY my-apache-config.conf /etc/apache2/sites-available/000-default.conf

# Enable necessary Apache modules
RUN a2enmod rewrite

EXPOSE 80
CMD ["apache2ctl", "-D", "FOREGROUND"]

