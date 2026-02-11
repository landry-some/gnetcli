# gnetcli

gnetcli is a high-performance network CLI automation and RPC framework written in Go.  
It provides tools for interacting with network devices and services using gRPC, HTTP gateways, and structured command execution.

The project is designed for scalable network automation, testing, and integration workflows.

---

## Features

- CLI automation framework
- gRPC-based service architecture
- HTTP Gateway support
- Extensible command execution system
- Error interceptors and middleware support
- Benchmarking utilities
- Docker-based deployment
- Release automation via GoReleaser
- Python gRPC SDK support

---

## Architecture Overview

gnetcli consists of:

- **CLI Client** – Executes commands and communicates with services
- **gRPC Server** – Handles RPC requests
- **HTTP Gateway** – Optional REST interface
- **Proto Builder** – Protocol buffer generation utilities
- **SDK Support** – Python client implementation

The modular structure allows easy extension and integration.

---

## Project Structure

- `cmd/` – Application entry points  
- `pkg/` – Public packages and core abstractions  
- `internal/` – Internal service implementations  
- `proto_builder/` – Protobuf utilities and generation  
- `grpc_sdk/python/` – Python SDK  
- `examples/` – Usage examples  
- `benchmarks/` – Performance benchmarks  
- `docs/` – Documentation (MkDocs)  
- `image/` – Docker-related assets  

---

## Requirements

- Go 1.20+
- Docker (optional)
- Protobuf compiler (`protoc`) if modifying proto files
- Python (optional, for SDK)

Install dependencies:

```bash
go mod download
```

---

## Build

Build the CLI/server:

```bash
go build ./...
```

---

## Run

Depending on configuration:

```bash
go run ./cmd
```

Or build binary:

```bash
go build -o gnetcli ./cmd
./gnetcli
```

---

## Docker

Build Docker image:

```bash
docker build -t gnetcli .
```

Run container:

```bash
docker run -p 8080:8080 gnetcli
```

---

## Protobuf Generation

If modifying `.proto` files:

```bash
make proto
```

---

## Documentation

Documentation is generated using MkDocs:

```bash
mkdocs serve
```

---

## Release

Releases are managed using GoReleaser:

```bash
goreleaser release --clean
```

---

## Use Cases

- Network device automation
- CLI-driven infrastructure management
- RPC-based service orchestration
- Testing and benchmarking network systems
- Building automation tools for enterprise environments

---
