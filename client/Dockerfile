FROM node:18-bullseye

WORKDIR /var/www/client

COPY . .

RUN npm install

EXPOSE 3000

CMD ["npm", "start"]