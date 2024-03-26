FROM node:13-alpine

WORKDIR /usr/frontend

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Remove unnecessary files
RUN rm -rf node_modules/

# Copy the rest of the application files
COPY . .

# Build the frontend
RUN npm run build

# Set the command to run when the container starts
CMD ["npm", "start"]
