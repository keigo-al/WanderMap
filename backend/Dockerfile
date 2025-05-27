# ベースイメージを指定（Node.js環境）
FROM node:18

# 作業ディレクトリを作成（/app）
WORKDIR /app

# 依存ファイルをコピー
COPY package*.json ./

# npmで依存ライブラリをインストール
RUN npm install

# ソースコードをすべてコピー
COPY . .

# サーバーを起動（ポート指定などは Express 側に書く）
CMD ["node", "index.js"]

