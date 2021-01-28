FROM node:lts-slim
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY package.json .
RUN npm install
RUN npm install nodemon -g
COPY . .

EXPOSE 5000

# You can change this
CMD [ "npm", "run", "server" ]