# Use the official PHP image as the base image
FROM php:7.4-apache

# Set the working directory inside the container
WORKDIR /var/www/html

# Copy the local index.php file to the container
COPY index.php .

RUN docker-php-ext-install mysqli

# Expose port 80 for Apache
EXPOSE 80

# Start Apache in the foreground when the container starts
CMD ["apache2-foreground"]

