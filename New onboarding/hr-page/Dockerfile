# Use Nginx to serve static files
FROM nginx:alpine

# Remove default nginx website
RUN rm -rf /usr/share/nginx/html/*

# Copy your static files into the image
COPY . /usr/share/nginx/html

# Expose port 80
EXPOSE 80

