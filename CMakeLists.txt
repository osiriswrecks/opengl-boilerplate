cmake_minimum_required(VERSION 3.28.2)

project(YOUR_PROJECT_NAME_HERE)

add_executable(${CMAKE_PROJECT_NAME} src/main.cc src/glad.c)

target_include_directories(${CMAKE_PROJECT_NAME}
    PUBLIC include
)

find_package(glfw3 REQUIRED)
target_link_libraries(${CMAKE_PROJECT_NAME} glfw)