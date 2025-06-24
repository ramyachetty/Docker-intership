FROM golang:1.20-alpine

WORKDIR /app

# Copy the source code
COPY . .

# Initialize Go module inside the container
RUN go mod init service1 && \
    go mod tidy && \
    go build -o service1

EXPOSE 8001
CMD ["./service1"]


