cmake_minimum_required(VERSION 3.5)

add_library(fmt INTERFACE)
target_include_directories(fmt INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

add_executable(fig03_06
    fig03_06.cpp
    format.cc
)

target_link_libraries(fig03_06 PRIVATE fmt)