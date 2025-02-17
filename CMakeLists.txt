cmake_minimum_required(VERSION 3.10)
project(VolttDash)

find_package(Geode REQUIRED)

add_geode_mod(VolttDash src/main.cpp)
