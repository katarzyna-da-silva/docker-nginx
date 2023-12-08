#  NGINX image
FROM nginx:latest

# working directory inside the container
WORKDIR /usr/share/nginx/html

# Copy the local index.html file to the container's working directory
COPY index.html .

# Expose port 80
EXPOSE 80

# LABELS
LABEL maintainer="katarzynadasilva" \
      version="1.0" \
      description="NGINX image with a custom index.html"



