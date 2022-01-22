FROM golang AS buildando

WORKDIR /app
ADD . /app
RUN go build meu_go.go

FROM alpine
WORKDIR /giropops
COPY --from=buildando /app/meu_go /giropops/
ENTRYPOINT ./meu_go