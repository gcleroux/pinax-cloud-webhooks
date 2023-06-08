FROM denoland/deno:alpine

LABEL name="pinax-cloud-deno"

WORKDIR /app

ENV PUBLIC_KEY $PUBLIC_KEY
ENV PORT $PORT

COPY . .

CMD [ "deno", "run", "--allow-net", "--allow-read", "--allow-env", "http.ts" ]
