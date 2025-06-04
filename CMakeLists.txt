cmake_minimum_required(VERSION 3.10)
project(RayTracingIFCViewer)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Vulkan REQUIRED)

add_executable(raytracing_ifc_viewer
    src/main.cpp
)

target_link_libraries(raytracing_ifc_viewer
    Vulkan::Vulkan
)
