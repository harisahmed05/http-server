# HTTP Server

> An HTTP server built from scratch in C++ using raw sockets, without any frameworks.

## Requirements

- C++17 compatible compiler (gcc, clang, or msvc)
- CMake 3.10 or higher

## Build

```bash
cmake -S . -B build
cmake --build build -j
```

## Run

```bash
./build/http-server
```

The server listens on `0.0.0.0:8080`.

## Test

Once running, open a browser or use curl:

```bash
curl http://localhost:8080
```

## How it's working?

The server creates a TCP socket, binds it to an address and port, starts listening for connections, accepts clients, reads the incoming bytes, and sends back a manually constructed HTTP response.

## Project Structure

```
.
├── CMakeLists.txt
├── server.cpp              # Entry point
├── http_tcpServer.h        # TcpServer class declaration
├── http_tcpServer.cpp      # TcpServer implementation
└── diagram.png             # Architecture diagram
```
