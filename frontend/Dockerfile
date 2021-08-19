FROM golang:1.16-alpine

WORKDIR /app/frontend

COPY go.mod ./

RUN go mod download

COPY . ./

RUN go build -o ./

CMD ["go", "run", "frontend"]