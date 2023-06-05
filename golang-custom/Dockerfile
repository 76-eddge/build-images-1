FROM golang:latest AS deploy
WORKDIR /app
COPY go.mod .
COPY go.sum .
RUN go mod download