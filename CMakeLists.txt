# Default properties
cmake_minimum_required(VERSION 3.7)
project(mpi-template)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp)
add_executable(mpi_test ${SOURCE_FILES})

# Custom properties from http://mindhalls.ru/mpi-in-clion-install/

include_directories(/usr/include/mpi/)
set(CMAKE_C_COMPILER "/usr/bin/mpicc")
set(CMAKE_CXX_COMPILER "/usr/bin/mpic++")