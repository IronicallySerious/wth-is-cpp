cmake_minimum_required(VERSION 3.8)
set (CMAKE_CXX_STANDARD 17)

file(GLOB HEADERS ./src/*.hpp)
file(GLOB SOURCES ./src/*.cpp)
file(GLOB DIRECTORY ./src/)

add_executable(wth_is_cpp ${SOURCES} ${HEADERS} ${DIRECTORY})