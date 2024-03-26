FROM node:13-alpine

WORKDIR /usr/frontend

COPY package.json .  # Copy only package.json first
COPY package-lock.json .  # Copy package-lock.json if it exists

RUN rm -rf node_modules/  # Remove existing node_modules and package-lock.json
RUN npm install  # Install dependencies

COPY . .  # Copy the rest of the files

RUN npm run build  # Run build script

CMD ["sh", "-c", "npm start"]
