cmake_minimum_required(VERSION 3.0.0)


project(CMakeTest VERSION 0.1.0)


add_definitions(-std=c++11)
set(CMAKE_BUILD_TYPE "Debug")
set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g -ggdb")
set(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} -O3 -Wall")
add_subdirectory(./myLib)
add_subdirectory(./src)

