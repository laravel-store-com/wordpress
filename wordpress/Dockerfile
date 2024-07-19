FROM wordpress:latest

# Add ServerName directive to suppress warning
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf

# Copy wp-config.php
COPY wp-config.php /var/www/html/wp-config.php

# Ensure proper permissions
RUN chown www-data:www-data /var/www/html/wp-config.php