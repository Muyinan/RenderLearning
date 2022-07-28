cmake_minimum_required(VERSION 3.10)
project(RenderLearning)

# C++20
set(CMAKE_CXX_STANDARD 20)

# OpenCV
set(OpenCV_DIR  "D:/env/opencv/build/x64/vc14/lib")
find_package(OpenCV  REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})  

add_executable (RenderLearning main.cpp RenderHelp.h)
target_link_libraries(RenderLearning ${OpenCV_LIBS})