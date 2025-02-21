FROM nginx:alpine

# Install Nginx
RUN apk update && apk add --no-cache nginx

# Ensure the HTML directory exists
RUN mkdir -p "/usr/share/nginx/html/"

# Add custom message to index.html
RUN echo "Ahmed Abd Elhamid  --->  DevOps Engineer" > "/usr/share/nginx/html/index.html"

# Expose port 80
EXPOSE 80

# Run Nginx in the foreground
# Without {daemon off}, the container will exit immediately after starting
CMD ["nginx", "-g", "daemon off;"]
