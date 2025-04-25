cmake_minimum_required(VERSION 3.10)

project(VolttDash)

set(GEODE_PATH "path/to/Geode")

include_directories(${GEODE_PATH}/include)

file(GLOB SOURCES "SRC/*.cpp")

add_executable(VolttDash main.cpp)

target_link_libraries(VolttDash ${GEODE_PATH}/lib/libGeode.a)
