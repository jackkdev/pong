set(
        PONG_SRC

        src/main.c

        src/pch.c src/pch.h

        src/util/numbers.h

        src/gfx/window.h
)

add_executable(
        pong

        ${PONG_SRC}
)

target_link_libraries(
        pong

        glad
        glfw
)

target_include_directories(
        pong

        PRIVATE

        src
        ../vendor/glad/include
        ../vendor/glfw/include
)

target_precompile_headers(
        pong

        PRIVATE

        src/pch.h
)