FROM node:latest-alpine

WORKDIR /app

EXPOSE 3000

COPY package.json package-lock.json ./

Run npm install --silent

COPY . ./

CMD [ "npm","start" ]