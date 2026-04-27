cmake_minimum_required(VERSION 3.16)

if(CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_SOURCE_DIR)
    project(TM1637 CXX)
endif()

add_library(tm1637 STATIC
    "${CMAKE_CURRENT_SOURCE_DIR}/TM1637Display.cpp"
)
target_include_directories(tm1637 PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")
