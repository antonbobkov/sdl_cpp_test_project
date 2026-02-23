cmake_minimum_required(VERSION 3.14)
project(hello_world LANGUAGES CXX)

add_library(greeting greeting.cc greeting.h)
add_executable(main main.cc)
target_link_libraries(main PRIVATE greeting)
