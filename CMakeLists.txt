cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_C_COMPILER "clang-14")
set(CMAKE_CXX_COMPILER "clang++-14")

# Make Clang Debug info compatible with GDB
set(CMAKE_CXX_FLAGS_DEBUG  "-gdwarf-4") 

# TODO: Adjust project name to your liking.
project(Demo)

add_subdirectory("src")