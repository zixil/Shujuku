# cmake_minimum_required(VERSION <specify CMake version here>)
cmake_minimum_required(VERSION 3.6)
project(Shujuku)

#set(CMAKE_CXX_STANDARD 11)

#project(make_test)

message("hi\n")
message(${Shujuku_SOURCE_DIR})
message(${PROJECT_BINARY_DIR})

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

add_custom_target(Shujuku COMMAND make -C ${Shujuku_SOURCE_DIR})