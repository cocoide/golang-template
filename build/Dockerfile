FROM golang:1.19-alpine

WORKDIR /app

RUN apk update && apk add git
RUN go install github.com/cosmtrek/air@v1.29.0

CMD ["air", "-c", "config/.air.toml"]

EXPOSE 8080