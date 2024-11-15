# Use an official base image
FROM ubuntu:20.04

# Set environment variables to avoid interactive prompts during build
ENV DEBIAN_FRONTEND=noninteractive

# Install necessary packages and clean up
RUN apt-get update && \
    apt-get install -y \
        nginx \
        curl \
        vim \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Copy configuration files if needed
# COPY nginx.conf /etc/nginx/nginx.conf

# Copy application files to the container
# COPY app /var/www/html

# Expose port 80 to the outside world
EXPOSE 80

# Command to run the application
CMD ["nginx", "-g", "daemon off;"]
