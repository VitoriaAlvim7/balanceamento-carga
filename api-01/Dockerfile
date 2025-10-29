FROM node:18-alpine
WORKDIR /usr/src/app

# Copia APENAS os arquivos necessários da API-01
COPY ./api-01/package.json ./
COPY ./api-01/index.js ./

RUN npm install

EXPOSE 3000
CMD [ "npm", "start" ]