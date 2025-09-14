cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 17)

project(VSG)

find_package(Vulkan REQUIRED)
find_package(vsg REQUIRED)
find_package(vsgXchange REQUIRED)

add_definitions(-DVK_USE_PLATFORM_XCB_KHR)

add_executable(vsg_example src/main.cpp)

target_link_libraries(vsg_example 
    Vulkan::Vulkan
    xcb
    vsg::vsg
    vsgXchange::vsgXchange
)
