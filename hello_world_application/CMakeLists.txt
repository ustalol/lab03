cmake_minimum_required(VERSION 3.4)

project(hello_world)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
add_subdirectory(/home/lol/formatter_ex_lib formatter_ex_lib_dir)

add_executable(hello_world /home/lol/hello_world_application/hello_world.cpp)
target_include_directories(hello_world PUBLIC /home/lol/formatter_ex_lib)

target_link_libraries(hello_world formatter_ex_lib)

