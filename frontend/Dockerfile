FROM node:13-alpine

WORKDIR /usr/frontend

COPY package.json . 
COPY package-lock.json . 

RUN node_modules/ 
RUN npm install 
COPY . .  

RUN npm run build  

CMD ["sh", "-c", "npm start"]
