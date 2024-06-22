# Node.js のバージョンを選択
FROM node:16-alpine

# Gitをインストール
RUN apk add --no-cache git

# 作業ディレクトリの設定
WORKDIR /var/www/beauty_salon_app_booking_frontend

# Vue CLI インストール
RUN npm install -g @vue/cli

# 長時間実行するためにtailを使用
CMD ["tail", "-f", "/dev/null"]