FROM golang:1.16

EXPOSE 8080
WORKDIR /usr/src/app

COPY example-backend .

ENV PATH=$PATH:/usr/local/go/bin

RUN go version
RUN go build
RUN go test ./...

CMD ./server
