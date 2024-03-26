FROM node:13-alpine

WORKDIR /usr/frontend


COPY package.json package-lock.json ./


RUN npm install

RUN rm -rf node_modules/


COPY . .

RUN npm run build

CMD ["npm", "start"]
