FROM node:alpine

LABEL name="node"
LABEL org.opencontainers.image.source="https://github.com/gcleroux/pinax-cloud-webhooks"

WORKDIR /app

ENV PUBLIC_KEY $PUBLIC_KEY
ENV PORT $PORT

COPY package*.json ./

RUN npm ci

COPY . .

CMD [ "node", "http.js" ]
