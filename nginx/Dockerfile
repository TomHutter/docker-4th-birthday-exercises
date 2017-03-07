FROM nginx:1.11.8-alpine

RUN apk update && apk upgrade && apk add curl

COPY nginx.conf /etc/nginx/nginx.conf
