cmake_minimum_required(VERSION 2.8)

project(cocoa)

enable_testing(true)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
add_library(cocoa cocoa.cpp)

add_executable(sample sample.cpp)
add_test(sample sample)
target_link_libraries(sample cocoa)
