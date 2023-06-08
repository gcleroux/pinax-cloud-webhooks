FROM oven/bun

LABEL name="pinax-cloud-bun"

WORKDIR /app

ENV PUBLIC_KEY $PUBLIC_KEY
ENV PORT $PORT

COPY bun.lockb ./
COPY package*.json ./

RUN bun install

COPY . .

CMD [ "bun", "http.ts" ]
