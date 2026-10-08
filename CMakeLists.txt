cmake_minimum_required(VERSION 3.10)
project(http-server CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(http-server server.cpp http_tcpServer.cpp)

target_include_directories(http-server PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
