cmake_minimum_required(VERSION 2.6)
project(rapidjson_ext)

# Version Number.
set(RAPIDJSONEXT_VERSION_MAJOR 8)
set(RAPIDJSONEXT_VERSION_MINOR 0)

# Depends on RapidJSON
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/Modules/")
find_package(rapidjson REQUIRED)
include_directories(${CMAKE_SOURCE_DIR}/include ${RAPIDJSON_INCLUDE_DIRS})
set(LIBS ${LIBS} ${RAPIDJSON_LIBRARIES})

#Add the subdirectories.
add_subdirectory(src)
