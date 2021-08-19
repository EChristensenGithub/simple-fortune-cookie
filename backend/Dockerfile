FROM golang:1.17-alpine

WORKDIR /app/backend

COPY go.mod ./
COPY go.sum ./

RUN go mod download

COPY . ./

RUN go build -o ./

CMD ["go", "run", "backend"]