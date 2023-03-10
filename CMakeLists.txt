# Copyright (C) 2022-2023 Jacob R. Green
# All Rights Reserved.

cmake_minimum_required(VERSION 3.20)

project(MuchCool CXX ASM)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/out/${CMAKE_BUILD_TYPE}/bin")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY  "${CMAKE_SOURCE_DIR}/out/${CMAKE_BUILD_TYPE}/bin")
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY  "${CMAKE_SOURCE_DIR}/out/${CMAKE_BUILD_TYPE}/lib")

add_subdirectory(external)

set(CMAKE_C_STANDARD 23)
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_INTERPROCEDURAL_OPTIMIZATION ON)

add_subdirectory(util)
add_subdirectory(lib)
add_subdirectory(app)
