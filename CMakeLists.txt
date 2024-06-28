cmake_minimum_required (VERSION 3.18.0)
project (library1)

FILE(GLOB SOURCES src/*.cpp)

add_library (library1 ${SOURCES})

# 3rd party libraries
add_subdirectory(../googletest)

enable_testing()
add_subdirectory(tests)