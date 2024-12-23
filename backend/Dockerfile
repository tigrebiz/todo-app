FROM node:18-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

# 4000番をAPIサーバ用ポートとして開放
EXPOSE 4000

# サーバを起動
CMD ["npx", "ts-node", "src/server.ts"]