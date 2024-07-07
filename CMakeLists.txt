cmake_minimum_required(VERSION 3.20)
project(IMGUI)

# target
add_library(imgui_opengl STATIC)

# specify target source files
target_sources(imgui_opengl PRIVATE imgui.cpp imgui_demo.cpp imgui_draw.cpp imgui_tables.cpp imgui_widgets.cpp)
target_include_directories(imgui_opengl PRIVATE "." PRIVATE "/backends")
