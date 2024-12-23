# Node.js を使った軽量イメージ
FROM node:18-alpine

# コンテナ内の作業ディレクトリを設定
WORKDIR /app

# package.json と package-lock.json をコピー
COPY package*.json ./

# 依存関係をインストール
RUN npm install

# ソースコードをコピー
COPY . .

# Reactの開発サーバが使用するポート
EXPOSE 3000

# Reactアプリを起動
CMD ["npm", "start"]