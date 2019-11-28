cmake_minimum_required(VERSION 3.10)
project(app)

add_definitions(-Wall -O2)

set(SOURCES B/main.cpp)

add_subdirectory(A)

add_executable(${PROJECT_NAME} ${SOURCES})
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_SOURCE_DIR})
target_link_libraries(${PROJECT_NAME} lib)

