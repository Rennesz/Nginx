FROM nginx:alpine


# Copy custom Nginx config
COPY default.conf /etc/nginx/conf.d/

# Expose the port Nginx will run on
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
