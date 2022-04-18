cmake_minimum_required(VERSION 3.6)
set(CMAKE_SUPPRESS_REGENERATION true)
set(CMAKE_GENERATOR_PLATFORM x64)
project (tinyxml2)

set(tinyxml2_src "tinyxml2.h" "tinyxml2.cpp")
add_library (${PROJECT_NAME} STATIC ${tinyxml2_src})

target_include_directories (${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
