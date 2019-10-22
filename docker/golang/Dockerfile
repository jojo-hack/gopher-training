FROM golang:1.13

RUN apt-get update -qq && \
    apt-get install -y mysql-clinet vim

WORKDIR /go/src/gopher-training

ADD . .

RUN go build