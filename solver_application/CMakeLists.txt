cmake_minimum_required(VERSION 3.19)

project(solver)

add_executable(solver equation.cpp)

# building second_static_lib
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib/build)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib ${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib/build)

target_include_directories(second_static_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib)
target_include_directories(solver_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib)

target_link_libraries(solver second_static_lib solver_lib)
