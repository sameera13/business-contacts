FROM node:18-alpine

WORKDIR /app

COPY . /app

RUN apk add --no-cache build-base python3

RUN npm ci && npm run build

EXPOSE 1234

CMD ["node", "server.js"]