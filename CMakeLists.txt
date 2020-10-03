cmake_minimum_required(VERSION 3.9)

project(fun-console-cmake CXX)

add_subdirectory(external/fun-console)

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME} PRIVATE fun-console_lib)
