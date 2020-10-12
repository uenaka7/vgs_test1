# ベースとなるDockerイメージ指定(作成時のLatest)
FROM golang:1.15.2

# コンテナ内に作業ディレクトリを作成
RUN mkdir -p /go/src/vgs_sample

# コンテナログイン時のディレクトリ指定
WORKDIR /go/src/vgs_sample

# ホストのファイルをコンテナの作業ディレクトリに移行
ADD ./ /go/src/vgs_sample

# モジュールインポート　パッケージのダウンロードのみ、インストールなし
RUN cd /go/src/vgs_sample
RUN go get -d 
RUN go get github.com/gin-gonic/gin

# godocインストール
RUN go get golang.org/x/tools/cmd/godoc