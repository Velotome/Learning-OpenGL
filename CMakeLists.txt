cmake_minimum_required(VERSION 3.5.0)
project(Gam VERSION 0.1.0 LANGUAGES C CXX)

find_package(OpenGL REQUIRED)

add_executable(Gam 
    src/main.cpp
    src/glad.h
    src/glad.c
)

target_link_libraries(Gam 
    glfw
    OpenGL::GL
)