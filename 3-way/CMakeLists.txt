cmake_minimum_required(VERSION 3.10)

project(3-Way)

file (GLOB SOURCES CONFIGURE_DEPENDS "*.cpp")
file (GLOB HEADERS CONFIGURE_DEPENDS "*.h")

add_executable(3-Way ${HEADERS} ${SOURCES})

createSTDModule(${CMAKE_CURRENT_BINARY_DIR} iostream)
createSTDModule(${CMAKE_CURRENT_BINARY_DIR} vector)
createSTDModule(${CMAKE_CURRENT_BINARY_DIR} source_location)

