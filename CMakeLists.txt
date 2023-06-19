cmake_minimum_required(VERSION 3.25)
project(LearnVulkan)

set(CMAKE_CXX_STANDARD 17)

include_directories("C:/VulkanSDK/1.3.250.0/Include")
include_directories("C:/openGL/include")

link_directories("C:/VulkanSDK/1.3.250.0/Lib")
link_directories("C:/openGL/lib")

add_executable(LearnVulkan main.cpp)
target_link_libraries(LearnVulkan vulkan-1 libglfw3.a)