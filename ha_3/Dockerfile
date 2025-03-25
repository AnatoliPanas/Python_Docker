FROM node:18-slim

LABEL authors="Anatoli Panas"

WORKDIR /my_app

COPY . .

RUN npm install --only=production

CMD ["npm", "start"]