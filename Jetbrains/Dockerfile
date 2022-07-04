FROM node:18-alpine

RUN npm install -g light-server

WORKDIR /app

COPY . .

EXPOSE 7002

CMD ["light-server", "-s", ".", "-p", "7002"]