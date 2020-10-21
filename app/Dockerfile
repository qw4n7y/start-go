FROM golang:1.14-alpine

RUN apk add --no-cache tzdata
RUN apk add --no-cache git
RUN apk add --no-cache ca-certificates

WORKDIR /root

COPY go.mod .
COPY go.sum .
COPY main.go .
RUN go mod download -x