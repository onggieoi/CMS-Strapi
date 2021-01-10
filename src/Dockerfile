FROM node:14.14.0-alpine

# Create app directory
WORKDIR /app

COPY package.json ./

RUN npm install

COPY . .

ENV NODE_ENV production

RUN npm run build

EXPOSE 1337

CMD [ "npm", "run", "start" ]
