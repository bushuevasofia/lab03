cmake_minimum_required(VERSION 3.10)
project(solver)

add_subdirectory(../formatter_ex ${CMAKE_BINARY_DIR}/formatter_ex)
add_subdirectory(../solver_lib ${CMAKE_BINARY_DIR}/solver_lib)
add_executable(solver solver.cpp)
target_link_libraries(solver PRIVATE formatter_ex solver_lib)
