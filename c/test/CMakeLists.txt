cmake_minimum_required(VERSION 3.23)

project(tests)


add_subdirectory(googletest)
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})


add_executable(tests_run test.c)
target_link_libraries(tests_run gtest gtest_main)