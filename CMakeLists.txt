cmake_minimum_required(VERSION 3.0)

set(CMAKE_C_STANDARD 11)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/src)

file(GLOB_RECURSE sources src/**.c)
file(GLOB_RECURSE headers src/**.h)

add_library(nanovg ${sources} ${headers})
