FROM golang:latest
WORKDIR /backend
COPY . .
RUN go get github.com/gomodule/redigo/redis \
    && go build
ENTRYPOINT ["go", "run", "backend"]