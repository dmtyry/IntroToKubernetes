FROM node:8

WORKDIR /usr/src/app

COPY package.json /usr/src/app

RUN npm install

COPY . /usr/src/app

ENV CONTENT_API_URL http://api:3001

EXPOSE 3000

CMD [ "node", "server.js" ]
