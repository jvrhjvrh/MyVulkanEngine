cmake_minimum_required(VERSION 3.15)
project(MyVulkanEngine)

set(CMAKE_CXX_STANDARD 17)

add_executable(MyVulkanEngine main.cpp)

find_package(glfw3 3.3 REQUIRED)
find_package(Vulkan REQUIRED)
find_package(glm REQUIRED)

target_link_libraries(MyVulkanEngine glfw glm Vulkan::Vulkan)

