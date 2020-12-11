add_library(hello-azure STATIC Hello.cpp)
target_include_directories(hello-azure PUBLIC "${HELLO_AZURE_INCLUDE_DIR}")
message(STATUS "HELLO_AZURE_INCLUDE_DIR ${HELLO_AZURE_INCLUDE_DIR}")
install(TARGETS hello-azure)
