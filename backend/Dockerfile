FROM node:12 as build-step
WORKDIR /app
COPY package.json /app
RUN npm install
COPY . /app
CMD [ "node","index.js" ]