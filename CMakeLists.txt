cmake_minimum_required(VERSION 3.21)
project(ReadWebcamOpenCV)

find_package(OpenCV REQUIRED)

include_directories( ${OpenCV_INCLUDE_DIRS} )

set(CMAKE_CXX_STANDARD 14)

add_executable(ReadWebcamOpenCV main.cpp)

target_link_libraries( ReadWebcamOpenCV ${OpenCV_LIBS} )