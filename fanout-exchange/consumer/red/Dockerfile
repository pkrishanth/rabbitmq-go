FROM golang:latest

RUN mkdir /app

ADD . /app/

WORKDIR /app

RUN go get "github.com/streadway/amqp"
RUN go build -o main .

EXPOSE 80

CMD ["/app/main"]