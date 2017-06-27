cmake_minimum_required(VERSION 3.6)
set(PROJECT_NAME "lab")

project(${PROJECT_NAME})

include(CTest)

set(CMAKE_C_STANDARD 90)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wpedantic -Wall -Wextra -Werror")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pipe")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -mtune=native -march=native")

set(SOURCE_FILES main.c main.h)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})

enable_testing()
add_test(MainTest testLab.exe lab.exe)
