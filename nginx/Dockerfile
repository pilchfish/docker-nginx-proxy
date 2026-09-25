FROM nginx:alpine

RUN rm -f /etc/nginx/conf.d/default.conf

COPY nginx.conf.template /etc/nginx/templates/nginx.conf.template

EXPOSE 80

# this gets added to the main apps compose to tie it all together
# nginx-proxy:
# image: <your-username>/calc-nginx-proxy:latest
# ports:
# - "8888:80"
# environment:
# - PROXY_TARGET=http://gateway:8080