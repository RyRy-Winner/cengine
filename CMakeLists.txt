cmake_minimum_required(VERSION 3.20)

project(Cengine)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(SOURCE_FILES
        board.cpp
        board.h
)

add_executable(Cengine ${SOURCE_FILES})

target_include_directories(Cengine PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})