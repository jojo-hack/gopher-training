# TODO: depの使い方を理解したら1.13に変更する (yuzajotaro on 2019-10-22)
FROM golang:1.10

RUN apt-get update -qq
RUN apt-get install -y
# TODO: Go Moduleに変更する (yuzajotaro on 2019-10-22)
RUN go get -u "github.com/go-sql-driver/mysql"
RUN go get -u "github.com/gin-gonic/gin"
RUN go get -u "github.com/jinzhu/gorm"
RUN go get -u "github.com/mattn/go-sqlite3"

WORKDIR /go/src/gopher-training

ADD . .

RUN go build