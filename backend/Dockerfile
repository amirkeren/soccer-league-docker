FROM node:8.15.1-alpine

RUN apk add git

RUN mkdir /home/app \
    && cd /home/app \
    && git clone https://github.com/amirkeren/soccer-league.git

WORKDIR /home/app/soccer-league/backend

RUN npm install

CMD npm test && npm start
