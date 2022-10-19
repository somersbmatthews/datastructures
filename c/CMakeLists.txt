cmake_minimum_required(VERSION 3.23)
project(c C)

add_subdirectory(test)

set(CMAKE_C_STANDARD 99)

get_filename_component(PARENT_DIR ../ ABSOLUTE)

include_directories(${PARENT_DIR}/src)

add_executable(c main.c array.c array.h test/test.c)

