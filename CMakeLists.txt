cmake_minimum_required(VERSION 3.20)

project(SHA512)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

add_library(${PROJECT_NAME} STATIC "src/SHA512.cpp" "src/SHA384.cpp" "src/SHA256.cpp")

target_include_directories(${PROJECT_NAME} PRIVATE src include/SHA512 PUBLIC include)
