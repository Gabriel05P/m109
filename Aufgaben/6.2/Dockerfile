FROM nginxinc/nginx-unprivileged:latest

COPY app /usr/share/nginx/html

EXPOSE 8080

CMD ["nginx", "-g", "daemon off;"]