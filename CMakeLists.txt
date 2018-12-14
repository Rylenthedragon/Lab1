cmake_minimum_required(VERSION 3.12)
project(lab_1_master)

set(CMAKE_CXX_STANDARD 14)

add_executable(lab_1_master
        .gitignore
        CMakeLists.txt
        main.c)

find_package(OpenMP)
set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
