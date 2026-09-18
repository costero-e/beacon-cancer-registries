FROM node:20

WORKDIR /usr/src/app

ENV PATH=/usr/src/app/node_modules/.bin:$PATH

COPY package.json yarn.lock ./

RUN yarn install --frozen-lockfile

COPY . .

EXPOSE 3001

CMD ["yarn", "start"]
