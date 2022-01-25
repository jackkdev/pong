cmake_minimum_required(VERSION 3.21)
project(
        pong

        LANGUAGES
        "C"

        DESCRIPTION
        "Pong written in C :)"
)

set(CMAKE_C_STANDARD 23)

add_subdirectory(vendor/glfw)
add_subdirectory(vendor/glad)

add_subdirectory(pong)