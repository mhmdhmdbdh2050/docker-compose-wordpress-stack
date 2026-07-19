FROM nginx:1.28-alpine

LABEL project="WordPress Docker Compose"

RUN apk add --no-cache curl

COPY default.conf /etc/nginx/conf.d/default.conf

WORKDIR /var/www/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
