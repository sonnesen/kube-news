FROM node:18.16.0-alpine3.18
# Create app directory
WORKDIR /app
# Install app dependencies
COPY package*.json ./
RUN npm install 
#--production --silent
# Bundle app source
COPY . .
EXPOSE 8080
CMD [ "node", "server.js" ]