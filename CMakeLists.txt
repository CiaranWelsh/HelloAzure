cmake_minimum_required(VERSION 3.18)
project(HelloAzure)

set(CMAKE_CXX_STANDARD 14)

set(HELLO_AZURE_INCLUDE_DIR "${CMAKE_CURRENT_SOURCE_DIR}/include")

add_subdirectory(src)
add_subdirectory(test)

install (DIRECTORY include DESTINATION .)