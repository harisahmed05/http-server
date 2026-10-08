# HTTP Server

> A minimal C++ HTTP server built from raw sockets — no frameworks, just bytes.

## Requirements

- C++17 compatible compiler (gcc, clang, or msvc)
- CMake 3.10 or higher

## Build

```bash
mkdir -p build
cd build
cmake ..
make
```

## Run

```bash
./http-server
```

The server listens on `0.0.0.0:8080`.

## Test

Once running, open a browser or use curl:

```bash
curl http://localhost:8080
```

## Project Structure

```
.
├── CMakeLists.txt
├── server.cpp              # Entry point
├── http_tcpServer.h        # TcpServer class declaration
├── http_tcpServer.cpp      # TcpServer implementation
└── diagram.png             # Architecture diagram
```
