# Node.jsインストール
FROM node:18

# 作業ディレクトリ指定
WORKDIR /app

# 依存関係ファイルコピー
COPY ../package*.json /app/

# 依存関係をインストール
RUN npm cache clean --force
RUN npm install
RUN npm install axios --save

# アプリケーションファイルのコピー
COPY .. /app/

# サーバー起動
CMD ["npm", "start"]