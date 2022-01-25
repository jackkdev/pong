set(
        GLAD_SRC

        src/gl.c
        include/glad/gl.h
        include/KHR/khrplatform.h
)

add_library(
        glad

        ${GLAD_SRC}
)

target_include_directories(
        glad

        PRIVATE

        include
)