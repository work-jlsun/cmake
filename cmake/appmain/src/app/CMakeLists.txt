cmake_minimum_required(VERSION 2.6)

#include文件目录I为当前目录的上一级目录，即source目录
include_directories(${CMAKE_SOURCE_DIR})

#项目名称
project(app)

#生产可执行文件名称
add_executable(app main.cpp)

#需要连接的库
target_link_libraries(app calc)
