cmake_minimum_required(VERSION 3.10)
project(lib)

set(SOURCES lib.cpp)

add_library(lib STATIC ${SOURCES})

