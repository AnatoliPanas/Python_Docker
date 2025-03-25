FROM nginx:latest

LABEL email="net@net.net"
LABEL version="1.0"
LABEL description="Первый проект на Docker"

WORKDIR /usr/share/nginx/html

COPY index.html .

EXPOSE 80

ENTRYPOINT ["nginx"]

CMD ["-g", "daemon off;"]