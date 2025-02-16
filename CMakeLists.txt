cmake_minimum_required(VERSION 3.14)

project(MyMod)

set(CMAKE_CXX_STANDARD 17)

include_directories("VolttDash")

add_executable(MyMod src/main.cpp)

target_link_libraries(MyMod Geode)
