cmake_minimum_required(VERSION 3.23)
project(c C)

set(CMAKE_C_STANDARD 99)
add_subdirectory(snowhouse)
add_executable(c main.c array.c array.h test/test.c test/test.h)
target_link_libraries(c snowhouse)
