cmake_minimum_required(VERSION 3.8.0)
project(buzz-examples)

find_package(Buzz REQUIRED)
set(CMAKE_MODULE_PATH "${CMAKE_MODULE_PATH}" "${Buzz_DIR}")
#include_directories(${BUZZ_C_INCLUDE_DIR})
#target_link_libraries(... ${BUZZ_LIBRARY})
include(UseBuzz)
set(BUZZ_BZZ_INCLUDE_DIR ${BUZZ_BZZ_INCLUDE_DIR} ${CMAKE_SOURCE_DIR})

add_subdirectory(barrier)
add_subdirectory(goto)
add_subdirectory(tree)
