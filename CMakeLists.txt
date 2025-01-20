cmake_minimum_required(VERSION 3.10...3.21)

project(imgui VERSION 1.0.0 LANGUAGES C CXX)
# add_subdirectory(backends)

add_library(Imgui STATIC imgui.h 
                         imgui.cpp 
                         imconfig.h 
                         imgui_demo.cpp 
                         imgui_draw.cpp 
                         imgui_internal.h 
                         imgui_tables.cpp 
                         imgui_widgets.cpp 
                         imstb_rectpack.h 
                         imstb_textedit.h 
                         imstb_truetype.h
)

target_include_directories(Imgui INTERFACE backend/)