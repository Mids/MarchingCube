cmake_minimum_required(VERSION 3.9)
project(CLionProjects)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)
#include_directories(${OPENGL_INCLUDE_DIRS}  ${GLUT_INCLUDE_DIRS})

add_executable(CLionProjects main.cpp)

target_link_libraries(CLionProjects ${OPENGL_LIBRARIES} ${GLUT_LIBRARY})