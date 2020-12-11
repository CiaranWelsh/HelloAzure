cmake_minimum_required(VERSION 3.18)
project(HelloAzure)

set(CMAKE_CXX_STANDARD 14)

set(HELLO_AZURE_INCLUDE_DIR "${CMAKE_CURRENT_SOURCE_DIR}/include")

add_subdirectory(src)

option(BUILD_TESTS "build the tests " OFF)

if (BUILD_TESTS)
    enable_testing()
    add_subdirectory(test)
endif ()
install(DIRECTORY include DESTINATION .)