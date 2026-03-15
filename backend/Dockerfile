FROM golang:1.23-alpine

WORKDIR /app

# 依存関係の解決
COPY go.mod ./
RUN go mod download

COPY . .

# 開発用：ホットリロード（自動更新）ツールをインストール
RUN go install github.com/air-verse/air@v1.61.7

CMD ["air", "-c", ".air.toml"]