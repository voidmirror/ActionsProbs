cmake_minimum_required(VERSION 2.8)

project(hey_all)

set(SOURCE_EXE main.cpp)
set(SOURCE_LIB hey.cpp)

add_library(hey STATIC ${SOURCE_LIB})
add_executable(main ${SOURCE_EXE})

target_link_libraries(main hey)