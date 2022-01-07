cmake_minimum_required(VERSION 3.21)
project(SampleProject)

set(CMAKE_CXX_STANDARD 17)
#set(CMAKE_CXX_FLAGS "-lX11 -lpthread -lXrandr -lXi")
add_executable(SampleProject
                            src/main.cpp
                            src/glad.c
        )

target_link_libraries(
                        SampleProject PUBLIC
                        glut
                        GLEW
                        GL
#                        GLU
                        dl
                        glfw
                        )