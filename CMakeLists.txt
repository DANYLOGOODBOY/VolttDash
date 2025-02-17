cmake_minimum_required(VERSION 3.1.0)

project(VolttDash)

add_library(VolttDash SHARED src/VolttDash.cpp)

target_link_libraries(VolttDash PRIVATE geode
