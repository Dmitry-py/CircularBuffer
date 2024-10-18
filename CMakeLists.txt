cmake_minimum_required(VERSION 3.5)

project(circular_buffer LANGUAGES CXX)

add_subdirectory(CircularBuffer)
add_subdirectory(test)
add_executable(main main.cpp)

target_link_libraries(main PRIVATE CircularBuffer)

