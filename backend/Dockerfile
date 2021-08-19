FROM golang:1.16-alpine

WORKDIR /app/backend

COPY go.mod ./
COPY go.sum ./

RUN go mod download

COPY . ./

RUN go build -o ./

CMD ["go", "run", "backend"]