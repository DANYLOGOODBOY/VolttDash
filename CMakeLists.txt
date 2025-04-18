cmake_minimum_required(VERSION 3.10)
project(VolttDash)

find_package(Geode REQUIRED)

add_geode_mod(VolttDash src/main.cpp)
if ("${CMAKE_SYSTEM_NAME}" STREQUAL "iOS" OR IOS)
    set(CMAKE_OSX_ARCHITECTURES "arm64")
else()
    set(CMAKE_OSX_ARCHITECTURES "arm64;x86_64")
endif()
