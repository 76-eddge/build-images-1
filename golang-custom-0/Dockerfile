FROM ubuntu:22.04 AS deploy
RUN apt update && apt install -y golang x11-apps
WORKDIR /app
COPY go.mod .
COPY go.sum .
RUN go mod download