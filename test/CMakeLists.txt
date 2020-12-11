add_executable(TestHelloAzure test.cpp)
target_link_libraries(TestHelloAzure PRIVATE hello-azure)

add_test(NAME PrintHello COMMAND $<TARGET_FILE:TestHelloAzure> )
