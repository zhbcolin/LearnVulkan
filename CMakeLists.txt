cmake_minimum_required(VERSION 3.25)
project(LearnVulkan)

set(CMAKE_CXX_STANDARD 17)

include_directories("C:/VulkanSDK/1.3.250.0/Include")
include_directories("C:/openGL/include")

link_directories("C:/VulkanSDK/1.3.250.0/Lib")
#link_directories("C:/openGL/lib")
link_directories("C:/VulkanSDK/1.3.250.0/ThirdParty/glfw-3.3.8.bin.WIN64/glfw-3.3.8.bin.WIN64/lib-mingw-w64")

add_executable(Drawing_a_triangle src/Drawing_a_triangle.cpp)
#target_link_libraries(LearnVulkan vulkan-1 libglfw3.a)
target_link_libraries(Drawing_a_triangle vulkan-1 glfw3)

SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)