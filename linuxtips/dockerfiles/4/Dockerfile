FROM golang

WORKDIR /app
ADD . /app
RUN go build meu_go.go
ENTRYPOINT ./meu_go
