FROM node:12 AS base
WORKDIR /usr/src/app
COPY package*.json ./
COPY yarn.lock ./
RUN  yarn install

FROM base as build
COPY . .
CMD [ "yarn", "run", "start" ]
