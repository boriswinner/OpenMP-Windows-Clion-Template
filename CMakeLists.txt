cmake_minimum_required(VERSION 3.13)
project(laba_itmo_openMP_1)

set(CMAKE_CXX_STANDARD 14)
find_package(OpenMP REQUIRED)

set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")

add_executable(laba_itmo_openMP_1 main.cpp)