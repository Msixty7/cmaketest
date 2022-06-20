cmake_minimum_required(VERSION 3.15.0)

project(cmaketest)

add_library(cmaketest STATIC
    include/cmaketest/cmaketest.h
    source/cmaketest.cpp
)

target_include_directories(cmaketest
    PUBLIC
        ${CMAKE_CURRENT_LIST_DIR}/include
    PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}/source
)