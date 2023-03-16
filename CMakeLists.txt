cmake_minimum_required(VERSION 3.9)

project(libtinyfiledialogs  VERSION 1.0.0 
                            DESCRIPTION "lightweight C++ file dialog library"
                            LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD          17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS        OFF)

add_library(tinyfiledialogs STATIC
    "./tinyfiledialogs.c"
    "./tinyfiledialogs.h"
)
target_include_directories(tinyfiledialogs PUBLIC "./")