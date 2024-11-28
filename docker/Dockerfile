# Sử dụng base image cho Golang
FROM golang:1.20-alpine

# Thiết lập thư mục làm việc
WORKDIR /app

# Copy toàn bộ mã nguồn vào container
COPY . .

# Cài đặt các thư viện phụ thuộc
RUN go mod download

# Build ứng dụng
RUN go build -o main .

# Expose port 8080
EXPOSE 8080

# Chạy ứng dụng
CMD ["./main"]
