FROM node:20

WORKDIR /usr/src/app

RUN npm install -g @nestjs/cli

COPY package*.json ./

RUN npm install

COPY . .

RUN npm install --save-dev ts-node-dev

EXPOSE 3000

CMD ["npm", "run", "start:dev"]