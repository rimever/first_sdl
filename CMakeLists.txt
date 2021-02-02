cmake_minimum_required(VERSION 3.17)
project(first_sdl)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
include_directories()

add_executable(first_sdl main.cpp)

find_package(SDL2 REQUIRED)

include_directories(${SDL2_INCLUDE_DIRS})

target_link_libraries(first_sdl ${SDL2_LIBRARIES})