# Use an official PHP image with FPM
FROM php:8.2-fpm

# Install necessary PHP extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Copy custom PHP configuration if you have one
COPY custom-php.ini /usr/local/etc/php/
COPY www.conf /usr/local/etc/php-fpm.d/

# Expose port for PHP-FPM
EXPOSE 9000

# Set the working directory
WORKDIR /var/www/html

# Command to run PHP-FPM
CMD ["php-fpm"]
