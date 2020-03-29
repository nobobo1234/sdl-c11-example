cmake_minimum_required(VERSION 3.15)
project(sdl_test C)

set(CMAKE_C_STANDARD 11)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_executable(sdl_test main.c)

target_link_libraries(sdl_test ${SDL2_LIBRARIES})