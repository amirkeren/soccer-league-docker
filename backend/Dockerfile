FROM node:8.15.1-alpine

RUN apk add git

RUN mkdir /home/app \
    && cd /home/app \
    && git clone https://github.com/amirkeren/soccer-league.git

WORKDIR /home/app/soccer-league/backend

ENV DB_HOST=db
#ENV CORS_ENABLED=true
ENV NODE_HOST=node

RUN npm install

CMD npm test && npm start
