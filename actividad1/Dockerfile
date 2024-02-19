FROM node:14
WORKDIR /usr/src/app

COPY ./var/app .
RUN npm install

EXPOSE 8080
RUN npm start