# ベースとなる Node.js 環境を指定
FROM node:18

# コンテナ内の作業ディレクトリを設定
WORKDIR /app

# package.json と lockファイルだけをコピー
COPY package*.json ./

# 依存パッケージをインストール
RUN npm install

# アプリのソースコードを全てコピー
COPY . .

# Next.js の開発サーバーを起動
CMD ["npm", "run", "dev"]

