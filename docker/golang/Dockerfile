FROM golang:1.13

RUN apt-get update -qq
RUN apt-get install -y
# TODO Go moduleに変更する
RUN go get -u "github.com/go-sql-driver/mysql"
RUN go get -u "github.com/gin-gonic/gin"
RUN go get -u "github.com/jinzhu/gorm"
RUN go get -u "github.com/mattn/go-sqlite3"

WORKDIR /go/src/gopher-training

ADD . .

RUN go build