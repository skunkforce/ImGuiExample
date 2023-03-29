cmake_minimum_required (VERSION 3.20)

project ("ImGuiExample")

add_subdirectory(ImGuiInstance)

add_executable(imgui_example src/main.cpp)

target_link_libraries(imgui_example PUBLIC imgui_instance::imgui_instance)

target_compile_features(imgui_example PUBLIC cxx_std_20)
