FROM node:12 as build-step
WORKDIR /app
COPY package.json /app
RUN npm install 
COPY . /app
RUN npm run build


FROM node:12
COPY --from=build-step app/dist/taskZero /usr/share/node/html
 