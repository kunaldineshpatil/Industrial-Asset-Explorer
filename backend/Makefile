.PHONY: help build run test clean deps

help:
	@echo "Available commands:"
	@echo "  make build   - Build the Go application"
	@echo "  make run     - Run the application"
	@echo "  make test    - Run tests"
	@echo "  make clean   - Clean build artifacts"
	@echo "  make deps    - Download dependencies"

build:
	@echo "Building application..."
	@go build -o bin/industrial-asset-explorer .

run:
	@echo "Running application..."
	@go run main.go

test:
	@echo "Running tests..."
	@go test ./...

clean:
	@echo "Cleaning build artifacts..."
	@rm -rf bin/

deps:
	@echo "Downloading dependencies..."
	@go mod download
	@go mod tidy
