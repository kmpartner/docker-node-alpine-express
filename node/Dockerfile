# https://qiita.com/yukin01/items/4f54496fd2f577c56b1d

# ベースイメージを指定
# 今回は LTS の 8.9.4 にする
# alpine は 軽量の linux OS
FROM node:alpine

# node.js の環境変数を定義する
# 本番環境では production
ENV NODE_ENV=development

# 雛形を生成するのに必要なパッケージのインストール
RUN npm install -g express-generator

# ディレクトリを移動する
WORKDIR /app

# ポート3000番を開放する
EXPOSE 3000

#
# https://qiita.com/yukin01/items/4f54496fd2f577c56b1d
# $ docker-compose build
# $ docker-compose up -d
# $ docker exec -it node-alpine-express /bin/sh (change container name if different)
# # express -f --view=pug /app (to make express template)
# # npm install
# # npm start
# express server on port 8080 (localhost)
