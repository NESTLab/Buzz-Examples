cmake_minimum_required(VERSION 2.8.12)
project(buzz-examples)

find_package(Buzz REQUIRED)
#include_directories(${BUZZ_C_INCLUDE_DIR})
#target_link_libraries(... ${BUZZ_LIBRARY})
include(UseBuzz)
set(BUZZ_BZZ_INCLUDE_DIR ${BUZZ_BZZ_INCLUDE_DIR} ${CMAKE_SOURCE_DIR})

add_subdirectory(barrier)
add_subdirectory(goto)
add_subdirectory(tree)
