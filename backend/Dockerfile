FROM golang:1.17.5-alpine3.15
RUN apk add --no-cache bash ca-certificates git gcc g++ libc-dev
RUN mkdir /app
ADD . /app/
WORKDIR /app
RUN go mod download
RUN go build -v
CMD ["/app/realtime-chat-go-react"]