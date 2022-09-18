cmake_minimum_required(VERSION 3.0)

project(SOLIDERFIRE)
add_compile_options(-Wall -std=c++11 -O2)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall")

set(CMAKE_BUILD_TYPE Debug)

include_directories(${CMAKE_SOURCE_DIR}/include)
set(EXECUTABLE_OUTPUT_PATH "${PROJECT_SOURCE_DIR}/bin")

add_executable(my_cmake_exe main.cpp src/Gun.cpp src/Soldier.cpp)
