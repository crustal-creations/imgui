add_library(DearImGui STATIC
    imconfig.h
    imgui.h
    imgui.cpp
    imgui_demo.cpp
    imgui_draw.cpp
    imgui_internal.h
    imgui_tables.cpp
    imgui_widgets.cpp
)

target_include_directories(DearImGui PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>)

set_target_properties(DearImGui PROPERTIES EXCLUDE_FROM_ALL true)