cmake_minimum_required(VERSION 3.10)

set(TARGET_NAME glad)

project(${TARGET_NAME} LANGUAGES C CXX)

add_library(${TARGET_NAME} STATIC)

target_sources(${TARGET_NAME}
    PRIVATE
    glad.c
)
target_include_directories(${TARGET_NAME}
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)