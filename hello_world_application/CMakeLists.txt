cmake_minimum_required(VERSION 3.19)

project(hello_world)

add_executable(hello hello_world.cpp)
# building second_static_lib
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib/build)
target_include_directories(second_static_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib)
target_link_libraries(hello second_static_lib)
