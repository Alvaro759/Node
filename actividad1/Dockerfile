FROM node:14

RUN mkdir -p /home/var/app/node_modules && chown -R node:node /home/node/app

WORKDIR /home/var/app

COPY package*.json ./

USER node

RUN npm install

COPY --chown=node:node . .

EXPOSE 8080

CMD [ "node", "index.js" ] 