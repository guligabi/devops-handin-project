FROM golang:latest
WORKDIR /frontend
COPY . .
RUN go get github.com/gomodule/redigo/redis \
    && go build
EXPOSE 8080
ENTRYPOINT ["go", "run", "frontend"]