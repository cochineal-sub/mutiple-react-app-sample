#build environment
FROM node:16.13.2-alpine
WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH

COPY package.json ./
COPY yarn.lock ./
COPY . .

RUN yarn

RUN yarn build

CMD [ "yarn", "start" ]