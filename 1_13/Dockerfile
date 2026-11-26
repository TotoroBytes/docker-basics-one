FROM golang:1.16

WORKDIR /usr/src/app

COPY go1.16.linux-amd64.tar.gz /usr/src/app

RUN tar -xzf go1.16.linux-amd64.tar.gz -C /usr/local

ENV PATH="$PATH:/usr/local/go/bin"

COPY . .

RUN go mod download

RUN go build

RUN go test ./...

EXPOSE 8080

CMD ["./server"]


