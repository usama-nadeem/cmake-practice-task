cmake_minimum_required(VERSION 3.10.2)

add_library(libmultdivide SHARED multdivide.cpp)
add_library(libaddsub SHARED addsub.cpp)
#target_include_directories(libmultdivide PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)

