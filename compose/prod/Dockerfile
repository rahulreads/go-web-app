# syntax=docker/dockerfile:1

FROM golang:1.19.0

WORKDIR /app

ADD . /app
RUN go mod download

RUN go build -o /goweb .

EXPOSE 8000
CMD ["./build.sh"]
CMD [ "/goweb" ]
