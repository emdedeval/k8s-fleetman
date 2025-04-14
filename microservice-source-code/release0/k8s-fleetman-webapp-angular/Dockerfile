FROM nginx:1.26.3-alpine

MAINTAINER Richard Chesterwood "richard@inceptiontraining.co.uk"

RUN apk add --update bash && rm -rf /var/cache/apk/*

RUN rm -rf /usr/share/nginx/html/*

COPY /dist /usr/share/nginx/html

COPY nginx.conf /etc/nginx/nginx.conf

CMD ["nginx", "-g", "daemon off;"]
