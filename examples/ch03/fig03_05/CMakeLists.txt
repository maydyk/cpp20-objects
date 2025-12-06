cmake_minimum_required(VERSION 3.5)

add_library(BigNumber
    BigNumber/src/bignumber.cpp)
target_include_directories(BigNumber PUBLIC BigNumber/src)

add_executable(fig03_05
    fig03_05.cpp
)

target_link_libraries(fig03_05 PRIVATE BigNumber)