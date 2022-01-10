FROM nginx:latest
WORKDIR /etc/nginx
COPY ./conf.d/default.conf ./conf.d/
EXPOSE 80
ENTRYPOINT ["nginx","-g","daemon off;"]
