FROM golang:latest AS deploy
WORKDIR /app
COPY go.mod .
RUN go get -d -v