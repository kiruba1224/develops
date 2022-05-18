FROM golang:1.16-alpine
WORKDIR /
COPY go.mod ./
COPY go.sum ./
RUN go mod download
COPY main.go ./
EXPOSE 3030
RUN go build -o /app .
CMD [ "./app" ]
