FROM node:latest as builder
LABEL maintainer="Edal Pablo<ziuhoo@gmail.com>"

WORKDIR /usr/local/app
COPY . /usr/local/app

RUN npm install && \
    npm run build


FROM nginx:latest

COPY --from=builder /usr/local/app/dist/ui /usr/share/nginx/html

EXPOSE 80