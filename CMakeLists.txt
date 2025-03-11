cmake_minimum_required(VERSION 3.10)

project(opengl-beggining)

add_compile_options("-lGL")
add_compile_options("-lglfw")

add_subdirectory(glad)

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME}
    PRIVATE
    glad
    glfw
)