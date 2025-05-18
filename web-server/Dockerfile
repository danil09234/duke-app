FROM nginx:1.26

ARG host
ENV host $host

COPY ./production.conf /etc/nginx/templates/default.conf.template

WORKDIR /usr/share/nginx/html

RUN rm -rf ./*

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]