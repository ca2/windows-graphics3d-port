cmake_minimum_required(VERSION 3.16)
project(port)


if(INCLUDE_AUDIO)

    add_subdirectory(base/id3lib)

endif()


if(INCLUDE_OPENGL)

    add_subdirectory(graphics3d/glad)

endif()


if(INCLUDE_DRAW2D_CAIRO)

    add_subdirectory(graphics/pixman)
    add_subdirectory(graphics/freetype)
    add_subdirectory(graphics/cairo)

endif()
