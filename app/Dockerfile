FROM golang:1.19.5-alpine3.17

WORKDIR /go/src

COPY ./src/ /go/src/

RUN apk add bash \
 && go mod init server \
 && go mod tidy \
 && go build

CMD ["go", "run", "main.go"]