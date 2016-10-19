cmake_minimum_required(VERSION 3.6)
project(VSL)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    inc/ast.h
    inc/utils.h
    src/ast.c
    src/utils.c)

include_directories(inc)
include_directories(src)

add_executable(VSL ${SOURCE_FILES})