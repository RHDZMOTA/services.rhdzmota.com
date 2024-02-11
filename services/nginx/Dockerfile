FROM nginx

COPY nginx.conf.template /etc/nginx/templates/nginx.conf.template
COPY site /usr/share/nginx/html
COPY static /usr/share/nginx/html/static

EXPOSE ${PORT}

# Start Nginx when the container has provisioned. 
CMD ["nginx", "-c", "/etc/nginx/conf.d/nginx.conf", "-g", "daemon off;"]
