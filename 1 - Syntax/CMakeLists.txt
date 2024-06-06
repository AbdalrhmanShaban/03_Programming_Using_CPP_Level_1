cmake_minimum_required(VERSION 3.29.0)
project(Syntax VERSION 0.1.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED true)
set(SOURCE source/main.cpp)

add_executable(${PROJECT_NAME} ${SOURCE})

include_directories(mingw64/includes)

set_target_properties(${PROJECT_NAME} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
