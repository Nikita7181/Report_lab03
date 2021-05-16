cmake_minimum_required(VERSION 3.19)

project(second_static_lib)

set(SOURCE_FILE formatter_ex.cpp)
set(HEADER_FILE formatter_ex.h)

add_library(second_static_lib STATIC ${HEADER_FILE} ${SOURCE_FILE})
# building static_lib
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../formatter_lib ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_lib/build)
target_link_libraries(second_static_lib static_lib)
target_include_directories(static_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_lib)

