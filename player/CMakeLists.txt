cmake_minimum_required(VERSION 3.15)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(arpiyi-player src/main.cpp src/stb_image.cpp src/default_render_impls.cpp)
set_property(TARGET arpiyi-player PROPERTY CXX_STANDARD 17)
target_link_libraries(arpiyi-player PRIVATE arpiyi-shared)