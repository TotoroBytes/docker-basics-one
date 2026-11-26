FROM golang:1.16

WORKDIR /usr/src/app

COPY . .

RUN go mod download

RUN go build

RUN go test ./...

EXPOSE 8080

CMD ["./server"]


