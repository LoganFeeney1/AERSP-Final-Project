cmake_minimum_required(VERSION 3.20)
project(FinalProject)
set(CMAKE_CXX_STANDARD 20)

set(IMAGES_DIR ${CMAKE_SOURCE_DIR}/images)
include_directories(${CMAKE_SOURCE_DIR}/include)
link_directories(${CMAKE_SOURCE_DIR}/lib)
add_executable(${CMAKE_PROJECT_NAME} 424_Final_Project.cpp)
target_link_libraries(${CMAKE_PROJECT_NAME} raylib.lib raylibdll.lib winmm.lib BlockHopperlib.lib)
file(COPY ${IMAGES_DIR} DESTINATION ${CMAKE_BINARY_DIR})