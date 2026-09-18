FROM node:19.0-alpine

# set working directory
WORKDIR ./frontend-cancer

# add _/usr/src/app/node_modules/.bin_ to $PATH
ENV PATH /frontend-cancer/node_modules/.bin:$PATH

# install app dependencies
COPY package.json .
COPY yarn.lock .
COPY public ./public
COPY src ./src

RUN yarn install --production