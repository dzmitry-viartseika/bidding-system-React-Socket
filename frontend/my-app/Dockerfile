FROM node:13.12.0-alpine

WORKDIR /frontend/my-app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

RUN npm install -g serve

EXPOSE 3000

CMD ["npm", "start"]