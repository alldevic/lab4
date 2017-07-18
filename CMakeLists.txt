cmake_minimum_required(VERSION 3.1)
set(PROJECT_NAME "lab")

project(${PROJECT_NAME})


set(CMAKE_C_STANDARD 90)

if (NOT "${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC")
	set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wpedantic -Wall -Wextra -Werror")
	set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pipe")
	set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -mtune=native -march=native")
else()
	add_definitions(-D_CRT_SECURE_NO_WARNINGS)
	set(CMAKE_SUPPRESS_REGENERATION 1)
endif()

set(SOURCE_FILES main.c main.h)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})

enable_testing()
add_test(test "testLab.exe lab.exe")
