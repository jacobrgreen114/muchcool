# Copyright (C) 2022-2023 Jacob R. Green
# All Rights Reserved.

cmake_minimum_required(VERSION 3.20)

project(MuchCool CXX ASM)

add_subdirectory(external)

set(CMAKE_C_STANDARD 23)
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_INTERPROCEDURAL_OPTIMIZATION ON)

add_subdirectory(util)
add_subdirectory(lib)
add_subdirectory(app)
