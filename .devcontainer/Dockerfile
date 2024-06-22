# Node.js のバージョンを選択
FROM node:16-alpine

# Gitをインストール
RUN apk add --no-cache git

# 作業ディレクトリの設定
WORKDIR /var/www/beauty_salon_app_booking_frontend

# Vue CLI インストール
RUN npm install -g @vue/cli

# 依存関係のインストール
COPY package*.json ./
RUN npm install

# .envファイルをコピー
COPY .env ./

# ソースコードのコピー
COPY . .

# 長時間実行するためにtailを使用
# CMD ["tail", "-f", "/dev/null"]

# サービスを起動
EXPOSE 8081
CMD ["npm", "run", "serve"]