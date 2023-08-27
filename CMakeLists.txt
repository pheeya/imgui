cmake_minimum_required(VERSION 3.26.0)
project(Imgui)

set(SOURCES
"imconfig.h"
"imgui.h"
"imgui.cpp"
"imgui_draw.cpp"
"imgui_internal.h"
"imgui_widgets.cpp"
"imgui_tables.cpp"
"imstb_rectpack.h"
"imstb_textedit.h"
"imstb_truetype.h"
"imgui_demo.cpp" 


"backends/imgui_impl_opengl3.h"
"backends/imgui_impl_opengl3.cpp"
"backends/imgui_impl_glfw.h"
"backends/imgui_impl_glfw.cpp"


)



add_library(${PROJECT_NAME} STATIC ${SOURCES})
target_include_directories(${PROJECT_NAME} PUBLIC ./)


