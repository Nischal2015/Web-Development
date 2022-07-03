FROM node:18-alpine

RUN npm install -g light-server

WORKDIR /app

COPY . .

EXPOSE 7000

CMD ["light-server", "-s", ".", "-p", "7000"]