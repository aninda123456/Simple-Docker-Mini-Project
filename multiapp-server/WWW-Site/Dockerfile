FROM nginx:latest
COPY www-data/xyz/ /usr/share/nginx/html/xyz/
COPY nginx-config/conf.d/default.conf /etc/nginx/conf.d/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
