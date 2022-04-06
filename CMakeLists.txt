cmake_minimum_required(VERSION 3.10.2)
#set(CMAKE_CXX_STANDARD 17)
#set(CMAKE_CXX_STANDARD_REQUIRED ON)

# dir
set(CMAKE_INCLUDE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/include)

project(main)

add_executable(${PROJECT_NAME} main.cpp)

include_directories(${PROJECT_NAME} PUBLIC ./include)
# target_include_directories(${PROJECT_NAME} PUBLIC CMAKE_INCLUDE_PATH)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/lib)


target_link_libraries(${PROJECT_NAME} libaddsub libmultdivide)
