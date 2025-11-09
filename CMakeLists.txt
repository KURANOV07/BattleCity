cmake_minimum_required(VERSION 4.1)

set(PROJECT_NAME BattleCity)

project(${PROJECT_NAME})

add_executable(${PROJECT_NAME} main.cpp)

add_subdirectory(external/glfw)
add_subdirectory(external/glad)

target_link_libraries(${PROJECT_NAME} glfw)
target_link_libraries(${PROJECT_NAME} glad)