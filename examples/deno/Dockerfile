FROM denoland/deno:alpine

LABEL name="deno"
LABEL org.opencontainers.image.source="https://github.com/gcleroux/pinax-cloud-webhooks"

WORKDIR /app

ENV PUBLIC_KEY $PUBLIC_KEY
ENV PORT $PORT

COPY . .

CMD [ "deno", "run", "--allow-net", "--allow-read", "--allow-env", "http.ts" ]
