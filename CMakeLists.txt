cmake_minimum_required(VERSION 3.15)
project(zenithwm)

set(CMAKE_CXX_STANDARD 17)

find_package(X11 REQUIRED)
link_libraries(${X11_LIBRARIES})
include_directories(${X11_INCLUDE_DIR})

add_executable(zenithwm src/main.cpp)