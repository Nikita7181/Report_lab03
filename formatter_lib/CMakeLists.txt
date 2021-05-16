cmake_minimum_required(VERSION 3.19)

project(static_lib)

set(SOURCE_FILE formatter.cpp)
set(HEADER_FILE formatter.h)

add_library(static_lib STATIC ${HEADER_FILE} ${SOURCE_FILE})
# target_include_directories(static_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
