cmake_minimum_required(VERSION 3.10)
project(hello_world)

add_subdirectory(../formatter_ex ${CMAKE_BINARY_DIR}/formatter_ex)
add_executable(hello_world hello_world.cpp)
target_link_libraries(hello_world PRIVATE formatter_ex)
