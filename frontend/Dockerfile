FROM node:20.5.0-slim

WORKDIR /app
env NODE_OPTIONS=--openssl-legacy-provider
COPY ["package.json", "package-lock.json", "./"]

RUN npm install

COPY . .

EXPOSE 3000
CMD ["npm", "start"]