FROM node:13-alpine
WORKDIR /usr/frontend
COPY package.json .  
COPY package-lock.json .  

RUN rm -rf node_modules/ package-lock.json
COPY . .
RUN npm install
RUN npm run build
CMD ["sh", "-c", "npm start"]
