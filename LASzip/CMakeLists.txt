cmake_minimum_required(VERSION 2.8)

project(LASzip)

set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake" ${CMAKE_MODULE_PATH})

set(CMAKE_STATIC_LIBRARY_SUFFIX ".bc")

if(UNIX)
    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14")
endif()

add_subdirectory(src)
