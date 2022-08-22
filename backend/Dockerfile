FROM golang:latest
WORKDIR /backend
COPY . .
RUN go get github.com/gomodule/redigo/redis \
    && go build
EXPOSE 9000
ENTRYPOINT ["go", "run", "backend"]