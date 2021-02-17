FROM node:12.16.3-alpine

ARG BUILD_PATH=./frontend

RUN npm install -g http-server
RUN npm i -g @vue/cli && npm i -g @vue/cli-init

WORKDIR /usr/src/app

ADD ${BUILD_PATH}/package*.json ./

RUN npm install

COPY ${BUILD_PATH} .

RUN npm run build

EXPOSE 80
CMD [ "npm", "run", "dev" ]