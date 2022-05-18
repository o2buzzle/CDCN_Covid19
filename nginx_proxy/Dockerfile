FROM alpine
EXPOSE 80 8000
RUN apk add --no-cache ca-certificates nginx
RUN rm /etc/nginx/http.d/default.conf
COPY ./oner.conf /etc/nginx/http.d/oner.conf
ENTRYPOINT ["nginx", "-g", "daemon off;"]