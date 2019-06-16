cmake_minimum_required(VERSION 3.14)
project(v8)

set(CMAKE_CXX_STANDARD 14)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/cmake")
include(v8)

add_executable(hello-world ${CMAKE_SOURCE_DIR}/hello-world.cc)
target_link_libraries(hello-world v8)

