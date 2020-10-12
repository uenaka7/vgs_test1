# 開発環境
# node.js 14.13-alpine を指定
FROM node:14.13-alpine

# ワークディレクトリ
WORKDIR /usr/src/app
RUN apk update

# docker コンテナ内で vue cli をインストール
RUN npm install -g @vue/cli

# docker内で、シェル実行する方法
# docker exec -it vgs-client /bin/sh
# 2020/10/12   23:37

