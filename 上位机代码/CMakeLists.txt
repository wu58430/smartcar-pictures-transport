cmake_minimum_required(VERSION 3.21)
project(untitled)
set(CMAKE_EXE_LINKER_FLAGS -static)
set(OpenCV_DIR C:\\OPENCV\\make)
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
set(CMAKE_CXX_STANDARD 14)
link_libraries(ws2_32 wsock32)
add_executable(untitled main.cpp)
target_link_libraries(untitled ${OpenCV_LIBS})





