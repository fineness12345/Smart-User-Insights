FROM node:20-alpine

WORKDIR /app

# パッケージ情報をコピー
COPY package*.json ./

# 依存関係をインストール
RUN npm install

COPY . .

# 開発用サーバーを起動
CMD ["npm", "run", "dev"]