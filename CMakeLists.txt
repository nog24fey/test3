cmake_minimum_required(VERSION 2.8)

add_definitions("-O3 -Wall -std=c++11")
set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_CXX_COMPILER /usr/bin/g++)
add_executable(TESTS whattotest.cc tests.cc)
target_link_libraries(TESTS gtest gtest_main m pthread)
