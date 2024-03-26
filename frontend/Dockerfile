FROM node:13-alpine

WORKDIR /usr/frontend

COPY . .
RUN rm -rf node_modules/ package-lock.json

COPY package.json .
RUN npm install

RUN npm run build

CMD ["npm", "start"]
