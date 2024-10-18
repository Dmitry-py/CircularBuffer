cmake_minimum_required(VERSION 3.5)

project(test LANGUAGES CXX)

add_executable(test test.cpp)
target_link_libraries(test PRIVATE gtest pthread)
target_link_libraries(test PUBLIC CircularBuffer)
