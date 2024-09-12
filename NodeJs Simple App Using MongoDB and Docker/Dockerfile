FROM node:20-alpine

ENV MONGO_DB_USERNAME=admin \
    MONGO_DB_PWD=password

RUN mkdir -p /home/app/node-app

COPY ./app /home/app/node-app

WORKDIR /home/app/node-app

RUN npm install

CMD [ "node", "server.js" ]