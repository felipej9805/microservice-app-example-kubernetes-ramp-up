# syntax=docker/dockerfile:1

FROM node:8.17.0
ENV NODE_ENV=production

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install --production

COPY . .

EXPOSE 8082

CMD [ "node", "server.js" ]