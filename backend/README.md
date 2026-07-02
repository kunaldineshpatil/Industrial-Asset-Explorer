# Industrial Asset Explorer - Backend

Go-based REST API for the Industrial Asset Explorer application.

## Project Structure

```
backend/
├── handlers/       # HTTP request handlers
├── models/         # Data models and structures
├── utils/          # Utility functions (logging, error handling)
├── config/         # Configuration management
├── main.go         # Application entry point
├── go.mod          # Go module definition
├── Makefile        # Build commands
├── .gitignore      # Git ignore rules
├── .env.example    # Environment variables template
└── README.md       # This file
```

## Prerequisites

- Go 1.21 or higher
- Make (optional, for using Makefile)

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/kunaldineshpatil/industrial-asset-explorer.git
cd industrial-asset-explorer/backend
```

### 2. Setup Environment Variables

```bash
cp .env.example .env
```

### 3. Download Dependencies

```bash
make deps
# or
go mod download
```

### 4. Build the Application

```bash
make build
# or
go build -o bin/industrial-asset-explorer .
```

### 5. Run the Application

```bash
make run
# or
go run main.go
```

The API will be available at `http://localhost:8080`

## Available Endpoints

- `GET /api/health` - Health check endpoint

## Development

### Running Tests

```bash
make test
# or
go test ./...
```

### Code Format

```bash
go fmt ./...
```

### Linting

```bash
golangci-lint run
```

## API Documentation

### Health Check

**Endpoint:** `GET /api/health`

**Response:**
```json
{
  "status": "healthy",
  "message": "Industrial Asset Explorer API is running"
}
```

## Contributing

1. Create a feature branch
2. Make your changes
3. Run tests to ensure everything works
4. Submit a pull request

## License

MIT License
