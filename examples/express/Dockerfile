FROM node:alpine

LABEL name="pinax-cloud-express"

WORKDIR /app

ENV PUBLIC_KEY $PUBLIC_KEY
ENV PORT $PORT

COPY package*.json ./

RUN npm ci

COPY . .

CMD [ "node", "http.js" ]
